# GameFabio
Aluno: Felipe Biava Favarin
Turma: 3° Fase de Ciência da Computação

Aqui está o diagrama final do código, que difere do passado em aula, porém segue os requisitos:

[Personagem]^[Herói]
[Personagem]^[Monstro]
[<<Interface>>Coletável]^-.-[Item]
[Item]^[Arma]
[Item]^[Poção]
[Herói]->[Coletável]


[<<Abstract>>Personagem| nome:String; dano:int; vida:int; força:int|atacar(Personagem p, Coletavel item):void;defender(Personagem p):void;getVida():int]

[Herói|item:Coletável|usarPocao(Personagem p):void;soltarItem():void;pegarArma(Coletavel item, int dano):void;pegarPocao(Coletavel item, int vida]

[Monstro|item:Coletável|]

[<<Interface>>Coletável| pegar():void;descartar():void;usar():void]

[<<Abstract>>Itens|coletado: boolean|pegar():void;descartar():void;]

[Arma| dano:int|usar():void;]
[Poção| vida:int;|usar():void]

