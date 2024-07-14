**# SR_ff in verilog**


Changed Q=2'b00; to Q <= 1'b0; in the reset condition.

Changed Q<=q; to Q <= 1'b0; in the 2'b11 case to avoid the ambiguous and illegal state.

Added an assign statement to assign the output q as the complement of Q properly.

Added or posedge rst in the always block sensitivity list to synchronize the reset.


**THE OUTPUT:**


![Screenshot 2024-07-14 143625](https://github.com/user-attachments/assets/2998db76-1b32-4273-b647-70b53783b3d7)
