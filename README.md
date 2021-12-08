# lambda-Comparator
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Romariorfr/lambda-Comparator/blob/master/LICENSE) 

## Uma experiência com Comparator
Estudo focado no aprendizado de programação funcional e expressões lambda.


## Sobre o projeto
#### Problema:
* Suponha uma classe Product com os atributos name e price

```java

public class Product {

	private String name;
	private Double price;

	public Product() {

	}


```





Podemos implementar a comparação de produtos por meio da implementação da interface Comparable<Product> entretanto, desta forma nossa classe não fica fechada para alteração, pois se o critério de comparação mudar , prescisaremos alterar a classe Product. Então podemos usar o default method "sort da interface List": 
  


```java

	public static void main(String[] args) {
		List<Product> list = new ArrayList<>();

		list.add(new Product("TV", 900.00));
		list.add(new Product("Notebook", 1200.00));
		list.add(new Product("Tablet", 450.00));

		list.sort((p1, p2) -> p1.getName().toUpperCase().compareTo(p2.getName().toUpperCase()));

		for (Product p : list) {
			System.out.println(p);
		}

	}


```
  
  ## Documentação
  Comparator: 
	
	https://docs.oracle.com/javase/10/docs/api/java/util/Comparator.html
  
  Metodo sort na interface List: 
	
	https://docs.oracle.com/javase/10/docs/api/java/util/List.html
  
 
  # Autor

Romário Ferreira de Rezende

https://www.linkedin.com/in/romarioferreiradeveloper

  




