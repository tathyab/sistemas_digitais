/*
	TRABALHO: Piscar Leds na placa da ALTERA
	 * Douglas Rosa
	 * Maikon Pereira
	 * Tatiane Barbosa
*/

module leds(
	input CLOCK_50,
	output [0:0]LEDR
);
	
reg [32:0] cont1 = 0;
reg reg1 = 0;

assign LEDR[0] = ~reg1;
	
always@(posedge CLOCK_50)
	begin
		if(cont1 == 10000000) 
			begin
				reg1 <= ~reg1;
				cont1 <= 0;
			end
		//--	
		else 
			begin
				cont1 = cont1 + 1;
			end
		end  
		
endmodule
