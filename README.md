# Classes-de-um-jogo
Escrevendo as classes de um jogo 

codigo 

class Heroi:
    def __init__(self, nome, idade, tipo):
        self.nome = nome
        self.idade = idade
        self.tipo = tipo

    def atacar(self):
        # Dicionário para mapear os tipos aos ataques correspondentes
        ataques = {
            "mago": "usou magia",
            "guerreiro": "usou espada",
            "monge": "usou artes marciais",
            "ninja": "usou shuriken"
        }

        # Obtendo o ataque correspondente ao tipo do herói
        ataque = ataques.get(self.tipo, "usou um ataque desconhecido")

        # Exibindo a mensagem de ataque
        print(f"O {self.tipo} atacou usando {ataque}")


# Criando alguns heróis de exemplo
heroi1 = Heroi("Arthur", 30, "guerreiro")
heroi2 = Heroi("Merlin", 100, "mago")
heroi3 = Heroi("Bruce", 40, "monge")
heroi4 = Heroi("Ryu", 25, "ninja")

# Chamando o método atacar para cada herói
heroi1.atacar()  # Saída: O guerreiro atacou usando espada
heroi2.atacar()  # Saída: O mago atacou usando magia
heroi3.atacar()  # Saída: O monge atacou usando artes marciais
heroi4.atacar()  # Saída: O ninja atacou usando shuriken
