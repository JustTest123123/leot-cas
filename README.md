<h1 id="a9U5i">控制端</h1>

> 光谱数据的采集端

<h2 id="OGicS">光谱测量 mode  -> 参数配置模块</h2>

> 配置端

+ 积分时间
  - 累计采集时间
+ 平均次数
+ 数据读取
+ 数据显示
  - 实时光谱测量数据展示
  - 历史采集数据展示
+ 存储（数据格式 std），内容扩展可调整，文件名设置，角度信息设置（是文件名的一个因素？）

<h2 id="BrxiS">自动 mode  -> 采集端</h2>

> 调用光谱仪真正的采集

+ 电机转动控制（人工或者自动）
  - 人工模式：调试模式，输入或者点击调整角度
  - 自动模式：以设定好的时间或者频率执行
    * eg：n个周期，每个周期 x 度
+ 光谱饱和判断
  - 初始化时判断是否采集？
  - 到达某个角度时判断是否采集？



<h2 id="DzPYE">测量 mode</h2>

+ 时间可调  -> <font style="color:#DF2A3F;">某个时间段 测量？</font>
  - 固定平均次数
  - 固定测量时间
+ 时间不调  -> <font style="color:#DF2A3F;">光谱满足就一直测？</font>



<h1 id="RPR5H">计算端</h1>

> 光谱数据的计算和渲染
>
> 把现在的三步合成一步即可（QDOAS调用、中间文件处理、调用IDL生成最终文件）

<h2 id="j33ON">中间数据生成</h2>

+ QDOAS调用
+ 周期文件的判断（一个周期结束）、读取
+ 结果文件的展示

<h2 id="he6tj">中间数据的处理</h2>

sciatran处理中间文件

<h2 id="XHmIc">最终文件的生成和展示</h2>

+ 调用IDL库，生成最终文件   -> IDL的弹窗问题
+ 文件展示  -> 多个文件的展示





