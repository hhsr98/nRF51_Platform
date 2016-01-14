#写入GPIO
***
##函数声明
```
void gpio_write (uint8_t pin, uint8_t state);
```


***
##函数功能
设置 gpio 的状态 (非0 - 高电平或者 0 - 低电平)。

***
##函数参数
参数    | 数据类型   | 说明
:----- | :-------- | :------
*pin*    | uint8_t  | 引脚号
*state*   | uint8_t  | 要设置的引脚的状态
*返回值*  | void      | 无

***
###关于 *state* 参数

*state* 的数值|说明
:-------- | :------
非0 | gpio输出高电平
0|gpio输出低电平

***
##函数举例
```
	//当前函数
	void foo( void )
	{
		...
		
		/*将偏移量为18的引脚配置成高电平*/
		gpio_setup(18, 1);
		
		...
	}
```	
	