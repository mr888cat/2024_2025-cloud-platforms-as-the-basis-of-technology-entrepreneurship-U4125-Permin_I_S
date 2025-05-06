# Лабораторная работа №2 «Исследование Cloud Run»  
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FTMI](https://itmo.ru/ru/viewfaculty/87/fakultet_tehnologicheskogo_menedzhmenta_i_innovaciy.htm)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2024/2025  
Group: U4125  
Author: Permin Ivan Sergeevich
Lab: Lab2  
Date of create: 06.05.2025  
Date of finished:  06.05.2025  
  
## Ход работы  
## Создание сервиса Cloud Run  
Сначала я зашел в раздел Cloud Run. Там отображаются все доступные сервисы.  
![[Pasted image 20250506153233.png]]  
  
Затем я приступил к созданию Cloud Run из представленного дефолтного сервиса Hello. Указал порт 8080.  
![[Pasted image 20250506153427.png]]  
  
Сервис создался.
![[Pasted image 20250506153745.png]]

  
## Тестирование сервиса Cloud Run  
Затем я перешел по ссылке и убедился, что все работает.  
![[Pasted image 20250506153831.png]]  
  
## Смотрим логи и метрики  
Перешел в соответствующие разделы.  
В логах мы видим статус GET 200, что говорит об успехе.  
![[Pasted image 20250506154027.png]]  
  
В метриках мы видим различные графики.  
![[Pasted image 20250506154106.png]]  
![[Pasted image 20250506154125.png]]  
  
## Смена порта Cloud Run  
Я зашел в настройки и поменял порт с 8080 на 8090.  
![[Pasted image 20250506154236.png]]
Сервис был успешно запущен.  
  
  
## Переключение трафика  
Затем я переключил трафик, разделив его 50/50.  
![[Pasted image 20250506154758.png]]  
  
## Логи и метрики  
В логах видим наш порт 8090.
![[Pasted image 20250506154855.png]]  
  
## Удаление ресурсов  
В конце я все удалил.
