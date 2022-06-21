# Pesquisa

## Temas

### Polimorfismo e Sobrescrita

A sobrescrita é o fato de alterar a implementação do método da classe pai.\
Quando eu tenho uma classe pai que possui um método e minha classe filha\
sobrescreve o metodo da pai.\
Serve para instaciar o objeto de varias maneiras diferentes.
O polimorfismo seria o poder de referenciar um objeto filho pela sua classe
        
    public class Animal {
    public void fazerBarulho(){
    System.out.println("Barulho");
    }
    }
---
    public class Cachorro extends Animal{
    public void fazerbarulho(){
    System.out.println("Au Au");
    }

---
    public class Galinha extends Animal{
    public void fazerbarulho(){
    System.out.println("Có Có");
---
    public class Main {
    public static void barulho(Animal animal){
    animal.fazerBarulho();
    }
    public static void main(String[] args){
    Cachorro cachorro = new Cachorro();
    Galinha galinha = new Galinha();
    barulho(cachorro);
    }
    }


Referencias

https://cursos.alura.com.br/forum/topico-sobrescrita-polimorfismo-45795

https://www.youtube.com/watch?v=i1pml_HXFxE

      
###Herança
A herenaça permite criar novas classes a partir de classes ja existentes, aproveitando\
das caracteristicas na classe pai.
A palavra-chave usada para indicar herança é extends.

      public class pessoa{
      puclic String nome;
      public int idade;
      }
---
      public class Aluno Extends Pessoa{
      public String matricula;
      }
---
      public class Estudos{
      public static void maind(String [] args){
      Aluno aluno = new Aluno();
      aluno.nome("Aluno Esforçado");
      aluno.idade(20);
      aluno.matricula("123456");
      
      System.out.println("Nome: " + aluno.nome + "\n" + "Idade: " + aluno.idade + "\n" +
      "Matricula: " + aluno.matricula);
      }
      }

Referencias

https://www.devmedia.com.br/encapsulamento-polimorfismo-heranca-em-java/12991#:~:text=A%20heran%C3%A7a%20%C3%A9%20um%20mecanismo,e%20reaproveitamento%20de%20c%C3%B3digo%20existente.
  

###Encapsulamento

O encapsulamento serve pra controlar o acesso aos atributos e métodos de uma classe.\
É uma forma de proteger os dados manipulados dentro da classe, alem de definir onde podera\
ser manipulada.

    public class Pessoa{
    private String nome;
    private String sobrenome;
    private String dataNasc;
    private String rg;
    private String[] telefones;
    
    public String getNome(){
    return nome;
    }
    public void setNome(String n){
    nome = n;
    }
    public String getSobrenome(){
    return sobrenome;
    }
    public void setSobrenome(String s){
    sobrenome = s;
    }
    public String getDataNasc(){
    return dataNasc;
    }
    public void setDataNasc(String d){
    dataNasc = d;
    }
    public String getRg(){
    return rg;
    }
    public void setRg(String r){
    r = rg;
    }
    public String getTelefones(){
    return telefones;
    }
    public void setTelefones(String[] telefones){
    telefones[] = telefones;
    }
    }


Referencias:

https://www.devmedia.com.br/encapsulamento-polimorfismo-heranca-em-java/12991#:~:text=O%20Encapsulamento%20serve%20para%20controlar,sentido%20para%20um%20membro%20particular.
## Requisitos

- No mínimo 15 linhas sobre cada assunto
  - O que é?
  - Pra que serve?
- Adicionar trechos de código de cada assunto;
- Entregar em markdown (se necessário, consultar na internet formatação markdown)
- Inserir todas as referências utilizadas (vídeo, links...)
