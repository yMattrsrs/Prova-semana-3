# Prova-semana-3
Prova Pyton Infinity School


alunos = {}

def add_aluno():
    nome = input("Nome do aluno: ")
    matricula = input("Número de matrícula: ")
    alunos[matricula] = nome
    print("aluno adicionado com sucesso! Seja bem vindo!")

def rem_aluno():
    matricula = input(" matrícula do aluno a ser removido: ")
    if matricula in alunos:
        del alunos[matricula]
        print("Aluno removido com sucesso!")
    else:
        print("matricula não existe.")

def lista_alunos():
    print("Lista de alunos:")
    for matricula, nome in alunos.items():
        print(f"Número de matrícula: {matricula}, Nome: {nome}")

while True:
    print("\nEscolha uma opção:")
    print("1 - Adicionar aluno")
    print("2 - Remover aluno")
    print("3 - Visualizar todos os alunos")
    print("4 - Sair")
    opcao = input("Digite o número da opção")

    # Tive que ver uns 15 tutoriais diferentes pra entender oq era p fazer :) 
