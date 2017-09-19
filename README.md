Author:YTC
Mail:recessburton@gmail.com
Created Time: 2017.6.30

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>

Description：
	新提出的协议的Tossim仿真模拟实现.
	对比ORW版本:1.9.1

Change Log：
	V1.8 修改生成forwardlist时各个邻居节点加入时的次序，由单edc改成综合考察
	V1.7 a.新metric的计算方式，在生成forwardlist时依次加入
		 b.增加收发包的总次数计数，以便计算能耗
		 c.重传间隔调整，根据average Qs整数倍往上涨
		 d.metric考察的时长扩大到20*睡眠周期
		 e.修改链路质量Qs联合概率计算公式
	V1.6 TOSSIM仿真头文件TossimRadioMsg.h中，将other1,other2,other3域的类型由
	uint8_t扩展到uint16_t,以满足程序需求。
