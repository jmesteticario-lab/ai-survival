# ai-survival
AI-Survival/ ├── backend/ ├── frontend/ ├── build_all.sh ├── README_BUILD.md
```python
import sys
import getpass

Seu ID único permitido
AUTHORIZED_USER_ID = "dni20862592-ar"

def autenticar():
    print("=== Sistema AI Survival Apocalipse ===")
    user_id = input("Digite seu ID de usuário: ")
    if user_id != AUTHORIZED_USER_ID:
        print("ID inválido. Acesso negado.")
        sys.exit()
    else:
        print("Acesso permitido. Bem-vindo!")

def main():
    autenticar()
    # Aqui você coloca a lógica principal da sua AI / app
    print("\nExecutando o sistema offline...")

    # Exemplo simples: simular consulta
    while True:
        comando = input("\nDigite seu comando (ou 'sair' para fechar): ").strip().lower()
        if comando == "sair":
            print("Encerrando sistema.")
            break
        else:
            print(f"Processando comando: {comando}")
