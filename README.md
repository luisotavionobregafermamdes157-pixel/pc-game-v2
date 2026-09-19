name: Meu PC Windows

on:
  workflow_dispatch:

jobs:
  windows:
    runs-on: windows-latest

    steps:
      - name: Informações do Windows
        run: |
          echo "Windows virtual iniciado"
          systeminfo

      - name: Teste
        run: |
          mkdir C:\MeuPC
          echo Meu PC virtual está funcionando > C:\MeuPC\teste.txt
          type C:\MeuPC\teste.txt
