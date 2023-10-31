import random

# 生成一个1到10之间的随机数
secret_number = random.randint(1, 10)
attempts = 0

print("欢迎来到猜数字游戏！")
print("猜一猜我心里想的是哪个数字？")

# 限制最多猜3次
while attempts < 3:
    guess = int(input("请输入你猜的数字："))
    attempts += 1

    if guess == secret_number:
        print(f"恭喜你！你猜对了。这个数字就是{secret_number}！")
        break
    else:
        print("猜错了！")

if attempts == 3:
    print(f"很遗憾，你没有猜对。正确的数字是{secret_number}。")

print("游戏结束。谢谢参与！")# yaohuichangku
