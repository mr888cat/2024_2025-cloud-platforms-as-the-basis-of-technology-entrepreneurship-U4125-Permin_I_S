# Лабораторная работа №1 «Обзор Google Cloud и исследование основных сервисов»  
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FTMI](https://itmo.ru/ru/viewfaculty/87/fakultet_tehnologicheskogo_menedzhmenta_i_innovaciy.htm)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2024/2025  
Group: U4125  
Author: Permin Ivan Sergeevich
Lab: Lab1  
Date of create: 06.05.2025  
Date of finished:  06.05.2025  
## Ход работы  
## Создание Service Account  
Сначала я зашел в раздел IAM & Admin — Service Account и создал аккаунт с ролью Storage Admin. Это оказалось важным шагом, так как без выбранной роли возникнет ошибка доступа.  
![1 1 p](https://github.com/user-attachments/assets/9daa76ed-2b69-410f-86c4-45ed950bfd49)


## Создание Compute Engine  
Затем я приступил к созданию Compute Engine (виртуальная машина) с заданными характеристиками: Machine type e2-micro в режиме spot.  
![Pasted image 20250506150839](https://github.com/user-attachments/assets/5f9318e5-48af-41ca-a04e-7f4f5f87bd2c)

  
Машина создалась и заработала.
 
![Pasted image 20250506150921](https://github.com/user-attachments/assets/b4e058ce-c368-4426-8986-72fdbf3622c8)

## Подключение к машине через SSH  
Я подключился к машине и выполнил команды по созданию новой папки и копированию в нее необходимых файлов. Все прошло успешно и файлы были скопированы.  
![Pasted image 20250506151754](https://github.com/user-attachments/assets/c68dadc8-5fee-46aa-ae13-afc10ebb3d41)

  
## Смена роли на Compute Viewer  
Я перешел в раздел редактирования Service Account и установил новую роль —  Compute Viewer.  
![Pasted image 20250506152212](https://github.com/user-attachments/assets/b7dea903-deef-4c97-b853-c84c4654d18a)


Затем я опять подключился к машине, однако выполнить копирование файлов не вышло. С данной ролью мы видим ошибку AccessDeniedException 403 — не хватает прав.  
![Pasted image 20250506152651](https://github.com/user-attachments/assets/d9449869-55fd-4ddc-b5f6-ff9d09a9aa97)

## Удаление ресурсов  
В конце я все удалил.
![Pasted image 20250506153008](https://github.com/user-attachments/assets/29020041-1322-4d59-88dd-d5064ffbfa00)
