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
![Pasted image 20250506153233](https://github.com/user-attachments/assets/fb2c5cd5-9413-489f-9fb8-b72faac7e3f4)

Затем я приступил к созданию Cloud Run из представленного дефолтного сервиса Hello. Указал порт 8080.   
![Pasted image 20250506153427](https://github.com/user-attachments/assets/d8c8e9e3-8dbe-4e56-840c-43c05ea41be4)

Сервис создался.
![Pasted image 20250506153745](https://github.com/user-attachments/assets/f42000c1-33a1-4b5a-8698-4946ab5d272a)

  
## Тестирование сервиса Cloud Run  
Затем я перешел по ссылке и убедился, что все работает.  
![Pasted image 20250506153831](https://github.com/user-attachments/assets/84a6becb-c48f-48ee-a09e-1cb01983e07d)

  
## Смотрим логи и метрики  
Перешел в соответствующие разделы.  
В логах мы видим статус GET 200, что говорит об успехе.  
![Pasted image 20250506154027](https://github.com/user-attachments/assets/421316b6-59f4-4c74-8dc6-91ceb55f2456)

  
В метриках мы видим различные графики.  

![Pasted image 20250506154106](https://github.com/user-attachments/assets/8ffad533-c425-49c1-a638-aca52f675476)



![Pasted image 20250506154125](https://github.com/user-attachments/assets/49aaf4fa-80a6-4b1d-ae38-0f99d7ddd8ff)

  
## Смена порта Cloud Run  
Я зашел в настройки и поменял порт с 8080 на 8090.  

![Pasted image 20250506154236](https://github.com/user-attachments/assets/53386ada-cda3-4c9e-9902-1770f811947f)

Сервис был успешно запущен.  
  
  
## Переключение трафика  
Затем я переключил трафик, разделив его 50/50.  

![Pasted image 20250506154758](https://github.com/user-attachments/assets/8885cd4a-9059-418a-9108-bb3a4b018450)

  
## Логи и метрики  
В логах видим наш порт 8090.

![Pasted image 20250506154855](https://github.com/user-attachments/assets/0d20c48d-442e-4df3-933f-022819589be3)

  
## Удаление ресурсов  
В конце я все удалил.
