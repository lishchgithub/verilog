+ 逻辑模块

	+ if...else...:

		```verilog
		if (a>1)
			begin
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

		

