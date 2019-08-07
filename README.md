# Java
##learning java
###simple java class

>特点
1.类名称必须有意义，再怎么说，要让人家看的明白吧
2.类之中所有属性必须使用private封装，并提供setter,getter方法
3.类之中可以有多个构造方法，但是必须保留有一个无参数构造方法
4.类之中不允许出现任何输出语句，所有输出必须交给被调用处
5.类之中需要有一个可以取得对象完整信息的方法，一般叫做getInfo(),返回String型数据

####代码示例：

class Book {
    private String name;
    private int price;
    private int num;
    public Book() {
        
    }
    public Book(String na ,int pri, int n) {
        name = na;
        price = pri;
        num = n;
    }
    public book() {
        
    }
    public void setName(String n) {
        name = n;
    }
    public void setPrice(int p) {
        price = p;
    }
    public void setNum(int n) {
        num = n;
    }
    public String getName() {
        return name;
    }
    public int getPrice() {
        return price;
    }
    public int getNum() {
        return num;
    }
    public  int  getMonney(int price, int num) {
        return price*num;
    }
    public String getinfo() {
        return "书名:"+name+"\n"+
               "单价:"+price+"\n"+
               "数量:"+num+"\n";
    }
}

public class test2 {
    public static void main(String args[]) {
        Book monney = new Book("老人与海",20,3);
        System.out.println(monney.getinfo());
    }
}
