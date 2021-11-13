# About Git

## Secure Hash Algorithm

o SHA1 ou Secure Hash Alrogorithm(Algoritmo de dispersão seguro) é um conjunto de funções hash criptográficas desenvolvida pela NSA. SHA-1 produz um valor de dispersão de 160 bits conhecido como resumo da mensagem. Um valor de dispersão SHA-1 é normalmente tratado como um número de 40 dígitos.

*Por exemplo*:

a8a0fa51aab3460c6deb7e9dd1f1bd1964c5d6c3

Informação a qual você pode achar usando um

```
git show
```

---

# Untracked to Tracked flow

![Imgur](https://i.imgur.com/yEqdSVb.jpg)

### Essa chart representa todos os estágios que um arquivo ou repositório pode se encontrar até que esteja pronto para que seja feito o commit.

* Começando na adição do arquivo ou repositório fazendo com que esse arquivo saia do *Untracked* e comece a ser *Tracked* e Unmodified.

* Caso algum arquivo seja modificado ele vai para o estado de Modified 

* Quando tudo está pronto para ser enviado tanto os novos arquivos/repositórios que tenham sido adicionados ou os existentes que foram modificados, é preciso adicionar essas alterações com:

  ```
  git add *
  git add .
  
  Os acima são usados para adicionar tudo que foi modificado dentro daquele repositório
  ```

* Após as alterações serem adicionadas com sucesso você pode fazer o commit das mesmas com:

  ```
  git commit -m "message"
  ```

​		**Parâmetro -m é usado para adicionar uma mensagem ao commit**

* Feito o commit só falta puxar as alterações do local host para o servidor com:

  ```
  git push origin "nomedabranch"
  ```

---

# Objetos Fundamentais

### Temos 3 Objetos fundamentais que compõe o Git sendo elas:

#### Blobs

Que são compostos por:

* SHA1
* Tamanho
* Conteúdo

#### Tree

Que são compostas por:

* Blobs
* SHA1
* Nome dos arquivos/repositórios
* Tamanho

#### Commit

Que são compostos por:

* Parente
* Tree
* SHA1
* Autor
* Mensagem
* Timestamp