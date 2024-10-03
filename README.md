- 👋 Hi, I’m @PuspitaHelal
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
PuspitaHelal/PuspitaHelal is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
 DATA SEGMENT 
    TEXT DB 0AH, 0DH,"ENTER THREE INPUTS..$" ;
ENDS
CODE SEGMENT 
    START: 
    MOV AX,@DATA
    MOV DS,AX
    
    LEA DX,TEXT
    MOV AH,9
    INT 21H 
     
    MOV AH,1
    INT 21H
    
    SUB AL,30H
    
    MOV BL,AL
    MOV AL, 100
    MUL BL
    
    MOV CL,AL,
    
    MOV AH,1
    INT 21H
    
    SUB AL,30H
    
    MOV BH,AL
    MOV AL,10
    MUL BH
    
    MOV DL,AL
    
    ADD CL,AL 
    
    MOV AH,1 
    INT 21H
    
    SUB AL,30H
    
    MOV DH,AL
    
    ADD CL,DH
    
    MOV AX,4C00H
    INT 21H
ENDS
END START
