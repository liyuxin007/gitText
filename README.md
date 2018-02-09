# vuestudy
装饰器中的*x为关键参数**y为非关键参数
*x对应元组 **y对应字典
def a(z):
    def b(*x,**y):
        for i in y:
            print(i)
            print('这里是Y') 
        for i in x:
            print(i)
            print('这里是X') 
    print(z)
    return b

def b (x,y,z):
    print(x*y*z)
c = a(b) 
c(1,2,3,x=1,y=2,z=3)
