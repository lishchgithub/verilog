module para_demo(clk,reset,a,b);  

input               clk;  

input               reset;  

input    [3:0]      a;  

output   [3:0]      b;  

reg      [3:0]      tempa1,tempa2,b;  

always@(posedge  clk)  

begin  

if(!reset)begin  

tempa1 <= 0;  

tempa2 <= 0;  

b <= 0;  

end  

else begin  

tempa1 <= a + 1;  

tempa2 <= tempa1 + 1;  

b      <= tempa2 + 1;      

end  

end  

endmodule  