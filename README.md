# 2020322094 张传扬 计G202
# JAVA第一次实验：
# 1.实验内容
·要求：完成教材p110第四题关于PC、CPU、HardDisk等的模拟程序。
·附加要求：
类中定义不少于两个构造方法。每个类定义不少于2个属性，且属性的类型应该多样化；根据课堂中关于访问权限的内容，尝试定义属性的修饰符多样化，类中定义方法操作属性，避免直接通过“类对象.属性”的形式访问属性值；且定义的方法内应该有符合常理的逻辑判断；尝试把本次实验的多个类放置在不同的包中，体会修饰符private的用法。
# 2.实验方法
·先设置一个CPU对象，用public方法,int类型定义speed
public class CPU {
	private int speed;
	
	public int getSpeed() {
		return speed;
	}
	public void setSpeed(int speed) {
		this.speed = speed;
	}

}
·设置HardDisk对象
public class HardDisk {
	private int amount;
	public int getAmount() {
		return amount;
	}
	public void setAmount(int amount) {
		this.amount = amount;
	}
}
# 3.核心方法
·创建cpu和disk对象，输出程序
public class PC {
	
	CPU cpu;
	HardDisk disk;
	
	public void setCpu(CPU cpu) {
		this.cpu = cpu;
	}
	public void setDisk(HardDisk disk) {
		this.disk = disk;
	}
	void show() {
		// TODO Auto-generated method stub
		System.out.println("CPU Speed:"+cpu.getSpeed());
		System.out.println("Hard Disk:"+disk.getAmount());
	}

}
·设置Test主类，实例化cpu、disk、pc，给cpu的speed赋值和amount赋值。
public class Test {
	public static void main(String[] args) {
		CPU cpu = new CPU();
		cpu.setSpeed(2200);
		HardDisk disk = new HardDisk();
		disk.setAmount(200);
		PC pc = new PC();
		pc.setCpu(cpu);
		pc.setDisk(disk);
		pc.show();
	}
	

}
# 4.实验结果
CPU Speed:2200
Hard Disk:200
# 5.实验感想
  1.本次实验让我熟练构造方法，创建对象，方法的调用
  2.public和private的不同
  3.对JAVA这门课程产生了浓厚的兴趣
  
