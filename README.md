# Web Technologies #
## This is my first experience in markdown ##
###### So let's try to do something ######

Try to do **Bold** and *italic* text.
And test two types of lists\n
* Item 1
* Item 2
  * Item 2.a
  * Item 2.b
  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3.a
   1. Item 3.b

Add picture
   ![Hi](https://vignette.wikia.nocookie.net/life-is-strange/images/1/1a/Fc%2C550x550%2Cwhite.jpg/revision/latest?cb=20170413133044&path-prefix=ru)
Format: ![Ooops](url)

Some info about good DB 
[here](https://habrahabr.ru/post/254773/)

Andrew Ryan:

> “It was not impossible to build Rapture at the bottom of the sea. 
> It was impossible to build it anywhere else.” 

Code snippets
#### *One crazy idea to write web server on c++* ####
```c++
	for (;;) {
		// Принимаем входящие соединения
		client_socket = accept(listen_socket, NULL, NULL);
		if (client_socket == INVALID_SOCKET) {
			cerr << "accept failed: " << WSAGetLastError() << "\n";
			closesocket(listen_socket);
			WSACleanup();
			return 1;
		}
		
		result = recv(client_socket, buf, max_client_buffer_size, 0);

		std::stringstream response; // сюда будет записываться ответ клиенту
		std::stringstream response_body; // тело ответа

		if (result == SOCKET_ERROR) {
			// ошибка получения данных
			cerr << "recv failed: " << result << "\n";
			closesocket(client_socket);
		}
		else if (result == 0) {
			// соединение закрыто клиентом
			cerr << "connection closed...\n";
		}
		else if (result > 0) {
			// Мы знаем размер полученных данных, поэтому ставим метку конца строки
			// В буфере запроса.
			buf[result] = '\0';

			// Данные успешно получены
			// формируем тело ответа (HTML)
```
#### *And my nightmares (from Antick's home tasks)* ####
```prolog
PREDICATES
  factorial(unsigned, long)
CLAUSES
  factorial(1,1). % Факториал от 1 равен 1. 5.
  factorial(N,FN):─ % Чтобы вычислить факториал числа N, надо вычислить   
  NewN=N-1, % факториал числа N-1 и умножить его на N. 
  factorial(NewN,Ft), 
  FN = N*Ft. 
GOAL   
``` 
And the goal
`X=3, factorial(X,FX). `
Table

Время|Предмет|Вид занятий|ФИО преподавателя 
-----|-------|-----------|-----------------
9:00-10:30|Физкультура и спорт| - | - 
10:40-12:10|ФиЛ программирование|лк|Смольянинова В.А.
13:00-14:30|Системы тестирования ПО|лк|Басок Б.М.
14:40-16:10|Системы тестирования ПО|лаб|Басок Б.М.
16:20-17:50|Системы тестирования ПО|лаб|Басок Б.М.

Link to my friend's github:
@zobninatn
Emoji
:pig2::dash::dash:
