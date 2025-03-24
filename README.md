# Problema Reserva de Hotel - Java

Durante meus estudos sobre Tratamento de Exceções em Java, desenvolvi uma atividade prática relacionada a um sistema de reservas de hotel.

A implementação utilizou a estrutura try-catch para lidar com possíveis erros, como datas inválidas ou tentativas de reserva conflitantes. O bloco try foi aplicado ao processo de registro da reserva, enquanto o catch capturou exceções específicas, exibindo mensagens apropriadas ao usuário.

Esse exercício reforçou a importância do tratamento de erros na construção de sistemas mais seguros e estáveis, garantindo uma melhor experiência para o usuário e evitando falhas inesperadas.
# 
### Problema
Fazer um programa para ler os dados de uma reserva de hotel (número do quarto, data de entrada e data de saída) e mostrar os dados da reserva, inclusive sua duração em dias. Em seguida, ler novas datas de entrada e saída, atualizar a reserva, e mostrar novamente a reserva com os dados atualizados. O programa não deve aceitar dados inválidos para a reserva, conforme as seguintes regras:
- Alterações de reserva só podem ocorrer para datas futuras
- A data de saída deve ser maior que a data de entrada

<div align = "center">
  
| Reservation        |
|--------------------|
| - roomNumber : Integer <br> - checkin : Date <br> - chekout : Date |
| + duration() : Integer <br> + updateDates(chekhin : Date, chekout : Date) : void |

</div>



#
### Exemplos
```
Room number: 8021 
Check-in date (dd/MM/yyyy): 23/09/2019
Check-out date (dd/MM/yyyy): 26/09/2019 
Reservation: Room 8021, check-in: 23/09/2019, check-out: 26/09/2019, 3 nights

Enter data to update the reservation: 
Check-in date (dd/MM/yyyy): 24/09/2019 
Check-out date (dd/MM/yyyy): 29/09/2019
Reservation: Room 8021, check-in: 24/09/2019, check-out: 29/09/2019, 5 nights
```
```
Room number: 8021
Check-in date (dd/MM/yyyy): 23/09/2019
Check-out date (dd/MM/yyyy): 21/09/2019
Error in reservation: Check-out date must be after check-in date
```
### Exemplos

```
Room number: 8021
Check-in date (dd/MM/yyyy): 23/09/2019
Check-out date (dd/MM/yyyy): 26/09/2019
Reservation: Room 8021, check-in: 23/09/2019, check-out: 26/09/2019, 3 nights

Enter data to update the reservation:
Check-in date (dd/MM/yyyy): 24/09/2015
Check-out date (dd/MM/yyyy): 29/09/2015
Error in reservation: Reservation dates for update must be future dates
```
```
Room number: 8021
Check-in date (dd/MM/yyyy): 23/09/2019
Check-out date (dd/MM/yyyy): 26/09/2019
Reservation: Room 8021, check-in: 23/09/2019, check-out: 26/09/2019, 3 nights

Enter data to update the reservation:
Check-in date (dd/MM/yyyy): 24/09/2020
Check-out date (dd/MM/yyyy): 22/09/2020
Error in reservation: Check-out date must be after check-in date
```
____

