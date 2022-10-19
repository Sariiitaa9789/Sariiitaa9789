import java.util.Arrays;

public class ArrayDeEnteros {

	public static void main(String[] args) {
		//DECLARAMOS LAS VARIABLES
		
		int num = 0;
		int i = 1;
		int n = 1;
		//INICIAMOS LA FUNCION FOR DONDE DECIMOS QUE I ES MENOR O IGUAL QUE 10 DEBEMOS INCREMENTAR
        for(; i <= 10; i++)
        {
            num += i;
        }
        
        //DEBEMOS CREAR UN ARRAY DENOMINADO NUMEROS
        int numeros[] = new int[num];
        
        //INDICAMOS LA POSCICION DONDE METER LOS NUMEROS
        int pos = 0;
        
        //INICIAMOS OTRA FUNCION FOR DONDE DECIMOS QUE SI N ES MENOR O IGUAL A 10 DEBE INNCREMENTAR
        for(;n <= 10; n++)
        {
            Arrays.fill(numeros, pos, pos + n, n);
            
            pos += n;
        }
        //VEMOS EL ARRAY CON LOS NUMEROS
        String arrayStr = Arrays.toString(numeros);
        System.out.println("Array " + arrayStr);
    }
	}



