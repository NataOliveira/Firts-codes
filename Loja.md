//Exemplo loja
//Um dos meus primeiros programas após dar inicio ao meus estudos sobre programação.


#include <stdio.h>
#include <string.h>

   	char nome[40];
	char endereco [50];
	char telefone[15];
	char cpf [15];
	
	
	int camisa_preta =45,camisa_verde=30,camisa_azul=35;
	int calca_jeans=120,calca_legg=45,bermuda=50;
	int tenis_nike=270,tenis_supreme=500,tenis_adidas=250;
	
	int camisa;
 	int tenis;
 	int calca;
 	
 	int continuar;
	int camisa2, calca2, tenis2;
	float tl;
	float final;
	
	
	
int main (int argc, char const *argv[])
{
	
	printf ("**********************************\n");
	printf ("  *** Welcome To My Store  ***\n");
	printf ("**********************************\n");
	printf ("\n Opcoes de camisas: ");
	
	printf("\n\n 1---Camisa preta R$45,00\n 2---Camisa verde R$30,00\n 3---Camisa Azul R$35,00\n Escolha: ");
	scanf("%i", &camisa);
	
	switch (camisa){

		case 1 :
		 camisa = camisa_preta;
		 break;
		 case 2 :
		 camisa = camisa_verde;
		 break;
		 case 3 :
		camisa = camisa_azul;
		 break;
		 default :
		 	printf(" \n Nenhuma opcao selecionada");
	}
	
	
	
	printf( "\n Opcoes de Calcas: ");
		printf("\n\n 1---Calca jeans R$120,00\n 2---Calca legg R$45,00\n 3---Bermuda R$50,00\n Escolha:");
	scanf("%i", &calca);
	
		switch (calca){

		case 1 :
		 calca= calca_jeans;
		 break;
		 case 2 :
	calca = calca_legg;
		 break;
		 case 3 :
		 calca = bermuda;
		 break;
		 default :
		 	printf(" \n Nenhuma opcao selecionada");
	
}



printf( "\n Opcoes de Tenis: ");
printf("\n\n 1---tenis Nike R$270,00\n 2---Tenis Supreme R$500,00\n 3---tenis Adidas R$250,00\n Escolha:");
	scanf("%i", &tenis);
	
	switch (tenis){

		case 1 :
	tenis = tenis_nike;
		 break;
		 case 2 :
		 tenis = tenis_supreme;
		 break;
		 case 3 :
		 tenis = tenis_adidas;
		 break;
		 default :
		 	printf(" \n Digite um valor correspondente");
		 	break;
	

}

printf(" \n Deseja Adicionar mais um item ?\n");
printf(" \n 1- sim \n 2- nao \n Digite: ");
scanf ("%i", &continuar);

if (continuar == 1){
		
	printf( "\n Opcoes de camisas: ");
		printf("\n\n 1---Camisa preta R$45,00\n 2---Camisa verde R$30,00\n 3---Camisa Azul R$35,00\n Escolha: ");
	scanf("%i", &camisa2);
	
	switch (camisa2){

		case 1 :
		 camisa2 = camisa_preta;
		 break;
		 case 2 :
		 camisa2 = camisa_verde;
		 break;
		 case 3 :
		camisa2 = camisa_azul;
		 break;
		 default :
		 	printf(" \n Nenhuma opcao selecionada");
	}
	
	
	
	printf( "\n Opcoes de Calcas: ");
		printf("\n\n 1---Calca jeans R$120,00\n 2---Calca legg R$45,00\n 3---Bermuda R$50,00\n Escolha:");
	scanf("%i", &calca2);
	
		switch (calca2){

		case 1 :
		 calca2= calca_jeans;
		 break;
		 case 2 :
		calca2= calca_legg;
		 break;
		 case 3 :
		 calca2 = bermuda;
		 break;
		 default :
		 	printf(" \n Nenhuma opcao selecionada");
	
}

printf( "\n Opcoes de Tenis: ");
printf("\n\n 1---tenis Nike R$270,00\n 2---Tenis Supreme R$500,00\n 3---tenis Adidas R$250,00\n Escolha:");
	scanf("%i", &tenis2);
	
	switch (tenis2){

		case 1 :
		 tenis2 = tenis_nike;
		 break;
		 case 2 :
		 tenis2 = tenis_supreme;
		 break;
		 case 3 :
		 tenis2 = tenis_adidas;
		 break;
		 default :
		 printf(" \n Digite um valor correspondente");
		 break;
		 }
	
fgets (nome,40,stdin);
printf ("\nDigite seu nome:\n");
fgets (nome,40,stdin);
printf("Digite seu CPF:\n");
fgets(cpf,15,stdin);
printf ("Digite seu endereco:\n");
fgets (endereco,50,stdin);
printf("Digite seu telefone:\n");
fgets(telefone,15,stdin);


printf("\n\n\n******************************");
printf("\n-----NOTA----- \nNome: %sCPF: %sEndereco: %sTelefone: %s \n\n", nome,cpf,endereco,telefone);

tl = camisa+calca+tenis;
final = camisa2+calca2+tenis2;
printf( "TOTAL: %.2f",tl+final);
	
	printf("\nObrigado e volte Sempre");
	printf("\n******************************");
	
}

else {	
fgets (nome,40,stdin);
printf ("\nDigite seu nome:\n");
fgets (nome,40,stdin);
printf("Digite seu CPF:\n");
fgets(cpf,15,stdin);
printf ("Digite seu endereco:\n");
fgets (endereco,50,stdin);
printf("Digite seu telefone:\n");
fgets(telefone,15,stdin);

printf("\n\n\n******************************");
printf("\n-----NOTA----- \nNome: %sCPF: %sEndereco: %sTelefone: %s \n\n", nome,cpf,endereco,telefone);

float tl = camisa+calca+tenis;

printf( "TOTAL: %.2f", tl);
	
	printf("\nObrigado e volte Sempre");
	printf("\n******************************");

}

	return 0;
}
