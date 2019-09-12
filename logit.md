+ 逻辑模块

	+ if...else...:

		```verilog
		if (a>1)
		    begin //多语句需要begin以及end包裹
				s=a+1
				s=2*s
			end
		else if (a<1)
			a = a+1
		else
			begin
				if (b==1)
					s = s-1
			end
			
		```

		

	+ case:

		```verilog
		reg [15:0] rega;
		reg [9:0] result;
		case(rega)
			16'd0:result=10'b1;
			16'd1,
			16'd2:result=10'b10;
			default:result=10'b110;
		endcase
			
		```

		

+ loop module：
	+ forever
	+ repeat
	+ while
	+ for

+ 命名块的禁用：
	+ disable block_name;
	+ 可以禁用任何一个block块（实现break）功能
+ 循环生成块：
	+ generate，endgenerate

+ 声明临时变量（主要用于for循环）
	+ genvar i