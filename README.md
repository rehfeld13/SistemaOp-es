# SistemaOp-es
Nesse algoritmo crio um sistema que gera 3 opções de escolha para o usuário, sendo elas: Calcular um valor de um produto, Uma partida de futebol e a opção de sair do sistema.





programa
 // by Rehfeld13
{
	
	funcao inicio()
	{
		inteiro numero = 0, numero2= 0
		
		
		inteiro golsTime1, golsTime2
        	cadeia time1, time2
        	real valorEtiqueta

        	enquanto (numero!= 3){
	
		escreva("(1) CALCULAR PREÇO DO PRODUTO \n")
		escreva("(2) PARTIDA DE FUTEBOL \n")
		escreva("(3) SAIR \n \n")

		escreva ("Escolha uma opção: ")
		leia(numero)
		limpa() 
        	

        	escolha (numero)
          {
          	caso 1: 
          	     escreva("Informe o valor de etiqueta do seu produto: ")
          	     leia(valorEtiqueta)
          	     escreva ("\n")

          	     escreva("(1) Aperte 1 se deseja pagar a vista com dinheiro \n")
				escreva("(2) Aperte 2 se deseja pagar a vista com cartão de crétido \n")
				escreva("(3) Aperte 3 se deseja parcelar em 2x \n")
				escreva("(4) Aperte 4 se deseja parcelar em 3x \n \n")

				escreva ("Escolha uma opção: ")
				leia(numero2)
				limpa()

				escolha (numero2)
				{
					caso 1:
					escreva ("O valor do seu produto é : "+(valorEtiqueta * 0.90)+"\n \n")
					pare

					caso 2:
					escreva ("O valor do seu produto é : "+(valorEtiqueta)+"\n \n")
					pare

					caso 3:
					escreva ("O valor do seu produto é : "+(valorEtiqueta * 1.05)+"\n \n")
					pare

					caso 4:
					escreva ("O valor do seu produto é : "+(valorEtiqueta * 1.10)+"\n \n")
					pare
				
				
				}
          	     
          	     
          	     
          	     pare

          	caso 2: 
          	     escreva ("Você iniciou uma partida de futebol: "+ "\n")
	       escreva ("Escreva o primeiro time: ")
	       leia(time1)
	       limpa()
	       escreva("Escreva o número de gols do "+time1+ ": ")
	       leia(golsTime1)
	       limpa()

	       escreva ("Escreva o segundo time: ")
	       leia(time2)
	       limpa()
	       escreva("Escreva o número de gols do "+time2+ ": ")
	       leia(golsTime2)
	       limpa()

	       se (golsTime1>golsTime2){
	       	escreva ("Placar: "+time1+" "+golsTime1+" x "+golsTime2+" "+time2+ "\n")
	       	escreva ("O vencedor foi: "+time1+"."+"\n"+"\n")
	          }

	       	senao se (golsTime1<golsTime2){
	       		escreva ("Placar: "+time1+" "+golsTime1+" x "+golsTime2+" "+time2+ "\n")
	       	escreva ("O vencedor foi: "+time2+"."+"\n"+"\n")
	       	}
	       	
	       	senao se (golsTime1 == golsTime2){ 
	          escreva ("Placar: "+time1+" "+golsTime1+" x "+golsTime2+" "+time2+ "\n")
	       	escreva ("EMPATE"+"\n"+"\n")
	       	}
	       	pare
                    

                    caso 3:
                    escreva("Você saiu!")
          }

		
        	}


        	
	}
}
