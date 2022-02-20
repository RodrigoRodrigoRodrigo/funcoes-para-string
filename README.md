
public class Main {

	public static void main(String[] args) {

		String original = "abcde FGHIJ ABC abc DEFG   ";

		String s01 = original.toLowerCase(); // imprimi todas as letras em minusculo.
		String s02 = original.toUpperCase(); // imprimi todas as letras em maiusculo.
		String s03 = original.trim(); // o trim ele vai mantar a mesma String original, so que ele vai eliminar os espaços nos cantos da String.
		String s04 = original.substring(2); // ele vai pegar somente o caracter da posição 2(c) em diante e montar uma nova String com esses caracteres.
		String s05 = original.substring(2, 9); // ele vai pegar somente o caracter da posição 2(c) ate o 9(h).
		String s06 = original.replace('a', 'x'); // trocar sempre que achar o a minusculo, e troca sempre pelo x minusculo.
		String s07 = original.replace("abc", "xyz"); // troca sempre o abc minusculo pelo xyz minusculo.
		int i = original.indexOf("bc");  // eu quero saber qual é a primeira posição do substring bc, que aqui é a posição 1.
		int j = original.lastIndexOf("bc"); // eu quero saber qual é a ultima ocorrencia do bc, quue aqui é a posição 17.

		System.out.println("original -" + original + "-");
		System.out.println("toLowerCase -" + s01 + "-");
		System.out.println("toUpperCase -" + s02 + "-");
		System.out.println("trim -" + s03 + "-");
		System.out.println("substring -" + s04 + "-");
		System.out.println("substring -" + s05 + "-");
		System.out.println("replace ('a', 'x') -" + s06 + "-");
		System.out.println("replace (abc, xyz) -" + s07 + "-");
		System.out.println("indexOf -" + i + "-");
		System.out.println("lastIndexOf -" + j + "-");

		// -------------------------------------------------------
		System.out.println(" ");
		// -------------------------------------------------------
		/*
		 * o split recebe um separador entre parenteses e aiele vai gerar um vector com as partes do string recortada
		 * conforme o separador que voce informar, se eu chamo s.split, recebendo o espaço em branco como separador
		 * o split vai fazer o seguinte, ele vai pegar o String s, recortar ele em varias partes separadas por espaço
		 * e guardar o resultado em um vetor.
		 */
		
		String s = "potato apple lemon";
		String[] vect = s.split(" "); // o split é uma função que serve para recortar o String

		/*
		 * String word0 = vect[0]; String word1 = vect[1]; String word2 = vect[2];
		 *
		 * System.out.println(word0); System.out.println(word1);
		 * System.out.println(word2);
		 */

		System.out.println(vect[0]);
		System.out.println(vect[1]);
		System.out.println(vect[2]);
	}

}
