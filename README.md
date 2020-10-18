# Java-
Java课程作业项目仓库
# 阅读程序
```
package src;

public class CPU {
	int speed;

	void setSpeed(int m) {
		/*
		 * 将参数m的值赋值给speed
		 */
		speed = m;

	}

	int getSpeed() {
		/*
		 * 返回speed的值
		 */
		return speed;

	}
}
public class HardDisk {
	int amount;

	void setAmount(int m) {
		/*
		 * 将参数m的值赋值给speed
		 */
		amount = m;

	}

	int getAmount() {
		/*
		 * 返回amount的值
		 */
		return amount;

	}

}
public class Test {
	/*
	 * 创建CPU对象cpu
	 */
	public static void main(String args[]) {

		CPU cpu = new CPU();
		/*
		 * speed设置为2200
		 */
		cpu.setSpeed(2200);
		/*
		 * 创建HardDisk对象disk
		 */
		HardDisk disk = new HardDisk();
		/*
		 * amout设置为200
		 */
		disk.setAmount(200);
		/*
		 * 创建PC对象pc
		 */
		PC pc = new PC();
		/*
		 * 调用setCPU(CPU c)方法，调用时实参是cpu
		 */
		pc.setCPU(cpu);
		/*
		 * 调用setHardDisk(HardDisk h)方法，调用时实参是disk
		 */
		pc.setHardDisk(disk);

		pc.show();

	}

}
public class PC {
	CPU cpu;

	HardDisk HD;

	/*
	 * 用setCPU(CPU c)方法将参数c的值赋值给cpu
	 */
	void setCPU(CPU c) {

		cpu = c;

	}

	/*
	 * 用setHardDisk(HardDisk h)方法将参数h的值赋值给HD
	 */
	void setHardDisk(HardDisk h) {

		HD = h;

	}
	/*
	 * show()方法显示cpu的速度和硬盘的容量
	 */
	void show() {

		System.out.println("CPU速度:" + cpu.getSpeed());

		System.out.print("硬盘容量:" + HD.getAmount());

	}

} 
```
## 实验目的
用类描述计算机中CPU的速度和硬盘容量。

### 实验过程
1.首先进行框架设计，在Test主类下有CPU.HardDisk.PC三个分类，主类从分类中调取参数并设计和调用显示参数show()从而达到显示CPU速度以及硬盘容量的目的。

2.创建CPU类，创建参数speed,并创建方法getSpeed,用于之后为speed赋值。

3.创建HardDisk类，创建参数amount，创建方法getAmount,之后赋值。

4.创建PC类，同上创建参数amount,之后赋值。

### 核心方法
1.利用Eclipse进行源代码操作（编译 调试 运行）。

2.利用Github网站进行实验报告的汇总。

## 实验结果
CPU速度2200 硬盘容量200

## 实验感想
通过这次实验使我明白了如何进行代码的操作和处理，让我懂得了参数amount的使用方法，如何赋值，如何查询数据。在这一系列的实验中，我基本掌握了Java的编程规则、知识要点和一些小技巧，同时，因正确的编出程序而带来的成就感让我对编程更加感兴趣。对于在这些实验过程中，请教老师、同学互助、查阅资料等基本的学习方式，使我更加领悟到集体和团队的力量，也树立了敢于攻坚的信心。
编程的经验增加了。但是在上机调试的时候还是遇到了相当多的问题。很多的错误都很难体会，有的时候是输入的错误，这种错误还是比较容易找出来的。发现JAVA虽然看起来比C或C++要容易一点，但是由于它自身带有相当多的方法定义，这些个方法虽然不用我们自己再去编写了，但是需要花相当多的时间去记忆哪些方法是需要导入的，还有方法名都是非常重要的。
