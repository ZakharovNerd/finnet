# FinNet 

ЗАДАЧА:<br>
Дан граф анонимизированный граф транзакций между юридическими лицами России. 

В файле vertices.csv информация о юридических лицах 
id - id юридического лица 
main_okved - основной ОКВЭД юридического лица (https://ru.wikipedia.org/wiki/Общероссийский_классификатор_видов_экономической_деятельности) 
region_code - код региона юридического лица 
company_type - тип юридического лица 

В файле edges.csv информация об обороте между юридическими лицами, прошедшем через счета банка Точка 
id_1 - id первого юридического лица 
Id_2 - id второго юридического лица 
value - суммарный оборот между юридическими лицами, к которому применено некоторое линейное преобразование 
n_transactions - количество транзакций между юридическими лицами, к которому было применено некоторое линейное преобразование 
Обратите внимание на то, что ребра неориентированные! 

В файле ids.csv информация о наиболее крупных юридических лицах, для которых требуется восстановить ребра 
id - id юридического лица 

Справочная информация: 
Справочник оквэдов - https://regforum.ru/okved/ 

Из графа было удалено 100 000 ребер, смежных юридическим лицам из файла ids.csv. Ваша задача - восстановить удаленные ребра и отправить в проверяющую систему файл submission.csv, который содержит 100 000 строк в формате id_1, id_2, где 
id_1 - id первого юридического лица 
Id_2 - id второго юридического лица 

Для вашего удобства ссылка на baseline решение [ССЫЛКА] 

МЕТРИКА: 
Метрика по которой будет оцениваться ваше решение 
score = intersection(test, prediction) 

Помните, что по ходу соревнований вам доступен public leaderboard, в котором решение оценивается на 50% отложенной выборки.  
В качестве финального решения загрузите файл submission.csv, который будет оценен на private leaderboard на оставшихся 50% отложенной выборки. Итоговые результаты оцениваются только по private leaderboard. 
ТАК ЖЕ ВМЕСТЕ С ФИНАЛЬНОЙ ПОСЫЛКОЙ НЕОБХОДИМО ОТПРАВИТЬ ВОСПРОИЗВОДИМЫЙ КОД С ВАШИМ РЕШЕНИЕМ В ВИДЕ ZIP АРХИВА.  
 
Удачи! 
