1. Configuração incial
![alt text](<Captura de tela de 2025-06-27 12-37-02.png>)

O ideal é que seja feito com a tag `--global`, porém eu uso mais de uma conta, então para este projeto, não a mencionei.

2. Para criar um repositório local
```
mkdir projeto
cd projeto
```

No meu caso, já tinha feito via Github, e por usar Fedora, utilizo do GitKraken (paralelo ao Github Desktop) e VSCode. Mas se fosse o caso de fazer manualmente, seria similiar à:

![alt text](<Captura de tela de 2025-06-27 12-40-56.png>)
![alt text](<Captura de tela de 2025-06-27 12-43-53.png>)

3. Adicionar arquivos e fazer commit

Como criei o `README.md` via Github, houve conflito.

![alt text](<Captura de tela de 2025-06-27 12-48-03.png>)

A seguir, seria o primeiro commit, porém como se pode ver, deu erro porque já existia previamente mas apaguei somente via IDE, e é necessário excluir via CLI e fazer o processo manualmente.

```
rm README.md
```

Processo original:
```
echo "# Novo Readme" > README.md
ls
git status
git add README.md
git push origin main
ls
```

![alt text](<Captura de tela de 2025-06-27 13-20-25.png>)
![alt text](<Captura de tela de 2025-06-27 13-20-44.png>)

5. Conectar ao repositório não é possível já que comecei com ele, mas o correto seria:
```
git remote add origin https://github.com/Hisllaylla/exe-git-github.git
git push -u origin main
```
6. Criar e trabalhar em nova branch
![alt text](<Captura de tela de 2025-06-27 13-39-05.png>)
![alt text](<Captura de tela de 2025-06-27 13-40-08.png>)

7. Fazer merge da branch na main
![alt text](<Captura de tela de 2025-06-27 13-41-29.png>)