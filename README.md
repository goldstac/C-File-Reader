# 📁 File Reader
## A File Reader Made In C
```c
#include <stdio.h>
#include <stdlib.h>
int main() {
  FILE *file = fopen("data.txt","r");
  if (file == NULL) {
    return 1;
  }
  char data[256];
  while (fgets(data,sizeof(data),file)) {
    printf("%s",data);
  }
  fclose(file);
  return 0;
}
```
## To Run
## In Linux
### Use build.sh
```bash
chmod +x build.sh
./build.sh
```
### Or Just Type
```bash
gcc -o main main.c
```
## In Windows
### Also Same
```bash
gcc -o main main.c
```
