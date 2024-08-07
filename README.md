# Inicialização do Pygame
pygame.init()

# Configurações da tela
largura = 800
altura = 600
tela = pygame.display.set_mode((largura, altura))
pygame.display.set_caption("Jogo de Avião")

# Cores
branco = (255, 255, 255)
azul = (0, 0, 255)

# Loop principal do jogo
while True:
    # Verificação de eventos
    for evento in pygame.event.get():
        if evento.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    # Lógica do jogo

    # Atualização da tela
    tela.fill(branco)
    # Desenhar o avião (exemplo básico)
    pygame.draw.rect(tela, azul, (400, 300, 40, 20))  # Exemplo de um retângulo representando o avião

    pygame.display.flip()

