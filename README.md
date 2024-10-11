# SWE_2021_41_2024_2_week_6

### Week 6 Assignment
Summarizing the work I've done for the week4 and week5 assignment


## Week4 Assignment
- Link of Repsitory : `https://github.com/0x106053b/SWE_2021_41_2024_2_week_4`
- Code Description :
  ```
  def isHappy(n):
  n_list = []
  while True:
    if n == 1:
      return True
    else:
      temp = sum(int(x)**2 for x in list(str(n)))
      if temp in n_list:
        return False
      else:
        n_list.append(temp)
        n = temp
  ```
The code above is implementation of simple algorithm quiz for jupyter .ipynb file practice. 
User can implement the code by clicking the run button next to the code cell.

<hr>

## Week5 Assignment
![ass_week5_screenshot (1)](https://github.com/user-attachments/assets/54d9849d-266a-41fc-92fe-19eddc390a14)
- This images shows the process of setting up environment for Docker container.
- Code Description :
> ```
> docker exec ossp-container cat /etc/os-release
> ```
> - Check which OS is running on. We can check Ubuntu 24.04 is activated now.

>```
>docker exec ossp-container git --version
>```
> - Check the installed version of git.

> ```
> docker exec ossp-container python3 --version
> ```
> - Check the installed version of python3.

> ```
> docker inspect --format="{{ .HostConfig.Binds }}" ossp-container [/home/yewon/ossp_host_dir:/mnt/ossp_container_dir]
> ```
> - Check path of mounted directory of the specified container.
