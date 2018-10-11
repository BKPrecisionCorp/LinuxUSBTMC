#include <sys/ioctl.h>
#include <unistd.h>
#include <sys/types.h>
#include <sys/stat.h>
#include <fcntl.h>
#include <stdlib.h>
#include <stdio.h>

int main(void){
  
  int instr;
  char* ret;
  ret = malloc(32);
  instr = open("/dev/usbtmc0", O_RDWR);
  write(instr, "*idn?\n",6);
  read(instr, ret, 32);
  printf("%s\n",ret);
  return 0;

}
