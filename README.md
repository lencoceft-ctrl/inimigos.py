# --- SISTEMA DE INIMIGOS (NÍVEL 1) ---

inimigo_base = {
    "nome": "DataBug-Gray",
    "estagio": "Baby I",
    "vida": 5,
    "ataque": "Pequeno Erro (Glitch)",
    "recompensa": "2 XP"
}

def iniciar_combate(player, inimigo):
    print(f"Alerta! Um {inimigo['nome']} apareceu no Terreno Raso!")
    print(f"{player} usa Bolhas de Pixel!")
    
    # Lógica de vitória simples para o estágio inicial
    if inimigo['vida'] <= 5:
        print(f"Vitória! {inimigo['nome']} foi deletado.")
        print(f"Você ganhou {inimigo['recompensa']}!")

# Simulando a batalha
iniciar_combate("Qi-mon", inimigo_base)
# --- SISTEMA DE VÍRUS (NÍVEL 1) ---

inimigo_virus = {
    "nome": "Smog-Virus (Fumaça)",
    "estagio": "Baby I (Dados Corrompidos)",
    "aparencia": "Névoa cinza escura com pixels piscando",
    "vida": 3,  # Menos vida, mas difícil de tocar
    "habilidade": "Infectar (Lentidão)",
    "descricao": "Uma fumaça tóxica que tenta corromper o mini oceano."
}

def combate_virus(player, inimigo):
    print(f"O ar ficou pesado... Um {inimigo['nome']} surgiu da corrupção!")
    print(f"{player} dispara suas Bolhas de Pixel para dissipar a fumaça!")
    
    # O Qi-mon vence porque o vento das suas bolhas afasta a fumaça
    print(f"A fumaça {inimigo['nome']} foi dispersada pelo vento do {player}!")
    print("O terreno está limpo novamente.")

# Executando o encontro
combate_virus("Qi-mon", inimigo_virus)

