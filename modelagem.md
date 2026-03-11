# 6. Modele e implemente um método recursivo que recebe um inteiro zero ou positivo e retorna um String com o número em binário.

     String convBase2(int n) 

erro:
n<0

base:
se 0 retorna '0'
se 1 retorna '1'

recursão:
'convBase2(n//2)'+str(n%2)

cot:
divide por dois e pega o resto.

# 7. Modele e implemente um método recursivo que calcule o somatório dos números contidos em um ArrayList de inteiros, passado como parâmetro.

erro:
se array vazio
base:
se array com 1 elemento, retorna array[0]
recursivo:
n[0] + soma_array(array[1:])

# 8. Modele e implemente um método recursivo para encontrar o maior elemento de um ArrayList.

     int findBiggest(ArrayList<Integer> ar) 

erro:
se array vazio

base:
se array com 1 elemento, retorna array[0]

recursivo:
se array[0]>array[len(array)-1]
    array[len(array)-1] = array[0]
    
    return find_biggest(array[1:])

# 9. Implemente um método recursivo para determinar se um string ocorre dentro de outro.

   boolean findSubStr(String str, String match)

erro:
base:
se len(str) and len(match) == 0:
    return True
se len(str) < len(match):
    return False

recursivo:
se str[0], match[0]:
    findSubStr(str[1:], match[1:])
else:
    findSubStr(str[1:], match)
