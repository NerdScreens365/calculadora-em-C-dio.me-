#include <stdio.h>

int main(){
	
	char operacao;
	float num1, num2, resultado;
	
	printf("digite uma das operacoes a seguir:\n+ para soma\n- para subtracao\n* para multiplicacao\n/ para divisao\n%% para resto de divisao\n");
	scanf("%c", &operacao);
	
	printf("digite o primeiro valor da operacao:\n");
	scanf("%f", &num1);
	
	printf("digite agora o segundo:\n");
	scanf("%f", &num2);
	
	switch (operacao){
		
		case '+':
			resultado = num1 + num2;
			printf("o resultado: %.2f", resultado);
			break;
		
	
		case '-':
			resultado = num1 - num2;
			printf("resultado: %f", resultado);
			break;
	
		case '*':
			resultado = num1 * num2;
			printf("o resultado: %f", resultado);
			break;
	
		case '/':
			resultado = num1 / num2;
			printf("o resultado: %f", resultado);
			break;
	
		case '%%':
			resultado = (int)num1 % (int)num2;
			printf("o resultado: %f", resultado);
			break;
		defalt:
			printf("Operacao invalida");
	
	}
		
