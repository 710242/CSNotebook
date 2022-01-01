# Chapter 1 I/O

#### 這是期末考前重點整理，所以內容指包括一些小觀念及作法，*沒有要深度探討*

### 1.scanf

```c
int main(){
  int a;
  scanf("%d",&a);
}
```

### 注意
- 非char陣列之外的型態都要加上位置符
- 若變數有很多個請用迴圈然後直輸入進陣列位置
- 不要在"%d"後面加"\n"

### 2.getchar

```c
int main(){
  char ch;
  ch = getchar();
}
```

### 注意
- 可以使用"(ch = getchar()) != EOF"當做判斷式放入while或if
- getchar()會讀到使用者輸入enter為止，所以字串題要用char才能讀到空格

### 3.printf

```c
int main(){
  printf("%d %c %s %f\n", int, char, char[], float);

  printf("%o %x %u\n", 8, 16, 10);

  printf("%100d %-100d %.9f\n");

  printf("%ld %sd\n");
}
```

### 注意
- %s會自動讀到字串陣列結尾（可記可不記？）
- o x u 分別表示8進位 16進位 10進位（unsigned）
- 型態前面加數字是留n個空格，小數點後則是輸出到小數點第n位
- l 即是 long , s 即是 short

### 4.putchar

不要用putchar
