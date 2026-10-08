\# Bài 2: Quản trị Tường lửa UFW



\## Yêu cầu



\* Default deny incoming

\* Allow SSH port 22/tcp

\* Allow HTTP port 80/tcp

\* Allow Spring Boot port 8082/tcp

\* Không allow MySQL port 3306/tcp



\## Kiểm tra UFW



```bash

sudo ufw status verbose

```



\## Kết quả



```text

Status: active

Logging: on (low)

Default: deny (incoming), allow (outgoing), deny (routed)



To                         Action      From

\--                         ------      ----

22/tcp                     ALLOW IN    Anywhere

80/tcp                     ALLOW IN    Anywhere

8082/tcp                   ALLOW IN    Anywhere

```



Port `3306/tcp` không được mở trên UFW.



