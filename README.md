# timeCounter
Как сделать отчет времени на  JS
1.Ставим крайную дату,до которой расчитывается время (deadLine)
2.function getTimeRemaining(endtime) :
  В t расчитываем разницу между deadline и настоящим в мс.
  Выщитывает от туда часы,минуты,секунды.
  Возвращаем объект с временными данными.
3.function setClock(id,endtime)
  id- Айди обертки в которой лежит 3 div - hours/minutes/seconds.
  Получаем это div.
  setInterval(updateClock, 1000) :
    Повторяем каждую секунду обновление времени из getTimeRemaining(endtime).
    function addZero(num) :
      Определяет вывсти число с нулем = "09" или без "11"
    Если время на таймере закончилось - выставить 00:00:00.
4. setClock('timer', deadline); передаем название обертки (timer) и конечное время (deadline);
