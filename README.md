# Aplicativo que fala se o usuário é ou não maior de idade

## Recebe o nome e a idade do usuário

## Classe com os atributos
```
package com.maioridade;

public class Maioridade {

	// Atributos
	public String nome;
	public int idade;
	
}
```

## Classe principal
```
package com.maioridade;

// importar a classe JOptionPane;
import javax.swing.JOptionPane;

public class Principal {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
        
		// Instancia o objeto do tipo Maioridade
		Maioridade usuario = new Maioridade();
		
		// Declaração de variáveis
		String idade;
		
		//Algoritmo
		
		// Recebe o nome do usuário
		usuario.nome = JOptionPane.showInputDialog("Informe seu nome:");
		
		// Recebe a idade do usuário
	    idade = JOptionPane.showInputDialog("Informe sua idade:");
		
	    // Converte string para int
	    usuario.idade = Integer.parseInt(idade);
	     if (usuario.idade >= 18)
	    	 JOptionPane.showMessageDialog(null, usuario.nome + " é maior de idade.");
	     else
	    	 JOptionPane.showMessageDialog(null, usuario.nome + " é menor de idade.");
	}
}
```