# Задание 1

1. Вывод версии Terraform:
![Вывод версии Terraform](/images/terraform_version.png)

2. Для хранения личной секретной информации допускается использовать файл terraform.tfvars или *.auto.tfvars
Секретная информация выделена в красном прямоугольнике:
![Секрет](/images/terraform_secret.png)

4. Нельзя использовать имена контейнеров, которые начинаются с цифры. Пропущено имя ресурса docker_image.

5. Вывод docker ps 
![dockerps](/images/docker_ps_1.png)

   Вывод docker ps после изменения имени контейнера
![dockerps](/images/docker_ps_2.png)

Содержимое terraform.tfstate после terraform destroy
![dockerps](/images/tfstate.png)

8. Образ nginx:latest не удален по причине наличия ключа keep_locally = true  (If true, then the Docker image won't be deleted on destroy operation. If this is false, it will delete the image from the docker local storage on destroy operation.)

# Задание 2
Plan для создаваемого ресурса находится в файле task2_main.tf