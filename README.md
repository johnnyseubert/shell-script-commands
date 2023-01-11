# Comandos de terminal

## ls

`lista itens de um diretorio`

---

## ls -la

`lista itens e itens escondidos`

---

## ls -i

`lista itens com o inode (id) do arquivo`

---

## ls \*.txt

`lista todos os itens com a extensao .txt pode ser utilizado com outras extensoes sem problemas exemplo ls *.ts`

---

## ls -l

`lista os arquivos com suas permissões`

-  `r permissoes de leitura`
-  `w permissoes de escrita`
-  `x permissoes de execucao`

---

## exit

`fecha o terminal`

```bash
exit
```

---

## CTRL + SHIFT + T

`Abre uma nova aba do terminal`

---

## clear CTRL + L

`limpa o terminal`

---

## reset

`reinicia o terminal removendo o historico`

```bash
reset
```

---

## $SHELL

`variavel que mostra o endereco na maquina do shell`

```bash
echo $SHELL
```

---

## Comentarios `#`

```bash
# Comentario
```

---

## pwd

`Retorna o diretorio atual ou do aplicativo`

```bash
pwd  # /mnt/c/Users/jbseu/Desktop exemplo
```

---

## cd

`comando para trocar de pasta ou diretorio`

```bash
cd .. # volta um diretorio

cd ~ # vai para a raiz

cd $HOME # vai para a raiz equivalente ao ~

cd CAMINHO # vai para a pasta desejada

cd - # volta para o diretorio anterior como um historico
```

---

## rmdir rm

`remove um diretorio, remove um arquivo`

```bash
rmdir NOME_DA_PASTA # apaga a pasta se tiver vazia

rm  NOME_DO_ARQUIVO # apaga o arquivo

rm -rf teste # apaga a pasta e tudo que tiver dentro
```

---

---

# Comandos de programação

---

## echo print

`escrevem no terminal`

```bash
echo teste

print teste
```

---

## echo -e

`O -e serve para interpretar os caracteres especiais`

```bash
echo -e "Rodolfo Dirack\n teste"
```

---

## Criar Variavel

```bash
NOME="teste"

echo $NOME
```

---

## cat

`serve para escrever no terminal o que tem dentro do arquivo`

```bash
cat teste.txt # escreve o texto dentro do arquivo no terminal
```

---

## echo >>

`este simbolo >> serve para escrever dentro de um arquivo e se nao existir ele cria`

```bash
echo "texto" >> arquivo.txt

cat arquivo.txt
# texto
```

---

## chmod

`serve para alterar permissoes de arquivos`

```bash
#drwxr-xr-x

# d => representa o tipo do arquivo d significa diretorio
# l => representa um link
# - => representa um arquivo normal texto etc..

chmod u=rwx teste.txt
# u= permissoes para usuario de leitura escrita e execucao

chmod g=rwx teste.txt
# g= para grupo de rede

chmod o=rw script.sh
# o= outros usuarios
```

---

## touch

`cria um arquivo desejado`

```bash
# exemplo
touch teste.txt
touch teste.json
touch teste.ts
```

---

## dirname

`retorna apenas o caminho do arquivo`

```bash
# Variavel ARQUIVO="/home/johnny/text.txt"

dirname $ARQUIVO
# /home/johnny
```

---

## basename

`retorna apenas o nome do arquivo`

```bash
# Variavel ARQUIVO="/home/johnny/text.txt"

basename $ARQUIVO
# text.txt

basename $ARQUIVO .txt # remove a extensao do arquivo
# text
```

---

## history

`retorna o historico dos ultimos 2k de comandos`

```bash
# Executar um comando do historico
!NUMERO DO COMANDO NO HISTORICO

!! # executa o ultimo comando do historico

history | tail -5
#retorna apenas os ultimos 5 comandos do historico

history | tail -5 >> arquivo.txt
#salvo os ultimos 5 comandos em um arquivo
```

---

## mkdir

`server para criar pastas`

```bash
mkdir teste # cria a pasta teste

mkdir -p ./teste/teste2 # cria multiplas pastas dentro de outras
```

---

## mktemp

`server para criar aruivos temporarios`

```bash
mktemp # /tmp/tmp.UM_HASH_MALUCO_GERADO

mktemp ./tmp.XXXX # cria
```

---

##

``

```bash

```

---
