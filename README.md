# GameFabio

Aqui está o diagrama passado em aula:
[Personagem]^[Herói]
[Personagem]^[Monstro]
[<<Interface>>Coletável]^-.-[Item]
[Item]^[Arma]
[Item]^[Poção]
[Herói]->[Coletável]


[<<Abstract>>Personagem| nome:String; dano:int; vida:int; força:int|atacar(Personagem p):void;defender(Personagem p):void;]

[Herói|item:Coletável|usarItem():void]
[Monstro]

[<<Interface>>Coletável| pegar():void;descartar():void;usar():void]

[<<Abstract>>Item|usado: boolean|pegar():void;descartar():void;]

[Arma| dano:int|usar():void;]
[Poção| ganho:int;cheia:boolean|usar():void]

Porém, tive que mudar a parte do usarItem():void do Herói.

[<<Abstract>>Personagem| nome:String; dano:int; vida:int; força:int|atacar(Personagem p):void;defender(Personagem p):void;getVida():int]



Porém
