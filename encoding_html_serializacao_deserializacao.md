São representações em hexadecimal de algum caracter, 
para que o mesmo não tenha de ser colocado na URL, 
sob pena de não ser compreendido enquanto a URL é 
transmitida entre servidores, máquinas, etc.

Especificamente, 
%20 é equivalente a um espaço (código ASCII 20 (hexadecimal)) e 
%30 é o número zero (código ASCII 30). 

Números geralmente não são codificados em uma URL, 
pois podem ser livremente escritos. 
Símbolos e outros caracteres sim.

Dá-se a essa formatação na URL 
o nome de "Character Encode". 
É uma forma de representar bytes e 
caracteres especiais na URL. 

O primeiro, por exemplo, 32 em decimal, 
se fora escrito de forma literal, na URL, 
geraria erro.

O encoding também é útil para escrever, 
via html, 
caracteres especiais e 
especialmente aqueles cujo teclado não contém tal símbolo, por exemplo:

Meu arquivo teste.html contém a seguinte codificação

  &mdash; "Traga-me as batatas, sim?";
  &bull;  "Pão"
  &bull;  "Alho"
  &bull;  "Batatas"

O "&mdash;" é o encoding para o — (travessão, não tem atalho, que eu saiba, no teclado Br-ABNT2); 
o "&bull;" gera os Bullets (lista), como se sabe. 

Os encodings, dentro do html, sempre vêm precedidos de & (ampersand) e 
é sufixados por ponto e vírgula.

# REFERÊNCIAS
[Avro](https://www.tutorialspoint.com/avro/serialization_using_parsers.htm)
[Como serializar e desserializar (empacotar e desempacotar) JSON no .NET](https://docs.microsoft.com/pt-br/dotnet/standard/serialization/system-text-json-how-to?pivots=dotnet-6-0)
[Quora](https://pt.quora.com/O-que-significa-20-e-30-em-URL)
[What is the difference between parsing and serialization?](https://dev.to/coolshaurya/what-is-the-difference-between-parsing-and-serialization-543b)
[W3 Schools](https://www.w3schools.com/tags/ref_urlencode.asp)
