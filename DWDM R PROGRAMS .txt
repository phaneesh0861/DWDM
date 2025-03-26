#1st
a=as.integer(readline(prompt = "enter the first number:"))
b=as.integer(readline(prompt = "enter the second number:"))
sum=a+b
print(sum)
#2nd
a=as.integer(readline(prompt = "enter the first number:"))
b=as.integer(readline(prompt = "enter the second number:"))
diff=a-b
print(diff)
#3rd
a=as.integer(readline(prompt = "enter the first number:"))
b=as.integer(readline(prompt = "enter the second number:"))
product=a*b
print(product)
#4th
a=as.integer(readline(prompt = "enter the first number:"))
b=as.integer(readline(prompt = "enter the second number:"))
divide=a/b
print(divide)
#5th
num = as.integer(readline(prompt = "enter a number:"))
if(num%%2==0){
  print("number is even")
} else {
  print("number is odd")
}
#6th
names = c("siri","divya","ram")
age = c(23,24,24)
marks = c(88,89,88)
df = data.frame(names,age,marks)
mean(df$age)
mode(df$age)
median(df$age)
write.csv(df,"datafr.csv")
#7th
names = c("siri","divya","ram")
age = c(23,24,24)
marks = c(88,89,88)
df = data.frame(names,age,marks)
summary(df$age)
write.csv(df$age,"datafr.csv")
#8th
a <- as.integer(readline(prompt = "Enter first number :"))
b <- as.integer(readline(prompt = "Enter second number :"))
c <- as.integer(readline(prompt = "Enter third number :"))

if (a > b && a > c) {
  print(paste("Greatest is :", a))
} else if (b > c) {
  print(paste("Greatest is :", b))
} else{
  print(paste("Greatest is :", c))
}
#9th
names<-c("siri","mahi","chiru")
age<-c(23,24,25)
marks<-c(88,78,25)
df<-data.frame(names,age,marks)
IQR(df $age)
write.csv(df,"datafr.csv")
#10th
names<-c("siri","mahi","chiru")
age<-c(23,24,25)
marks<-c(88,78,25)
df<-data.frame(names,age,marks)
quantile(df $age)
write.csv(df,"datafr.csv")
#11th
names<-c("siri","mahi","chiru")
age<-c(23,24,25)
marks<-c(88,78,25)
df<-data.frame(names,age,marks)
max_val = max(df $age)
min_val = min(df $age)
mid_range = (max_val+min_val)/2
mid_range
write.csv(df,"datafr.csv")
#12th
diabetest1<-read.csv("C:/Users/sande/OneDrive/Desktop/WeightLoss.csv")
A<-c(diabetest1$wl2)
Mean<-mean(A)
Std<-sd(A)
Zscore<-(A-Mean)/Std
Zscore
#13th
diabetest1<-read.csv("C:/Users/sande/OneDrive/Desktop/WeightLoss.csv")
A<-c(diabetest1$wl2)
Mean<-mean(A)
Minimum<-min(A)
Maximum<-max(A)
MinMax<-(A-Minimum)/(Maximum-Minimum)

data <- data.frame(Mean,Minimum,Maximum,MinMax)
data
#14th
a<-c(55,67,89,80,90)
barplot(a)
a<-c(55,67,89,80,90)
barplot(a)
barplot(a,horiz=FALSE)
#15th
names<-c("siri","chru","loki")
age<-c(23,24,25)
marks<-c(88,78,25)
df<-data.frame(names,age,marks)
hist(df$age)
boxplot(df$age)
#16th
a<-c(55,67,89,80,90)
hist(a)
#17th
diabetest1<-read.csv("C:/Users/sande/OneDrive/Desktop/WeightLoss.csv")
diabetest1<-table(diabetest1$wl1,diabetest1$wl2)
diabetest1
chisq.test(diabetest1)
#18th
set.seed(9)
x <- rnorm(1000)
y <- rnorm(1000)
smoothScatter(y - x)
smoothScatter(x,y)
#19th
library(ggplot2)
set.seed(123)
data <- data.frame(
  x = rnorm(100),
  y = 2 * rnorm(100) + 3
)
model <- lm(y ~ x, data = data)
summary(model)

ggplot(data, aes(x = x, y = y)) +
  geom_point() +
  geom_smooth(method = "lm", se = FALSE) +
  labs(title = "Linear Regression",
       x = "X",
       y = "Y")
#20th
library(ggplot2)

set.seed(123)
data <- data.frame(
  x1 = rnorm(100),
  x2 = rnorm(100),
  y = 2 * rnorm(100) + 3
)

model <- lm(y ~ x1 + x2, data = data)

summary(model)
ggplot(data, aes(x = x1, y = y)) +
  geom_point() +
  geom_smooth(method = "lm", se = FALSE) +
  labs(title = "Multiple Regression",
       x = "X1",
       y = "Y")






