function INC(input){return input+1;} 
function DEC(input){return input-1;} 
let counterReducer=[INC,DEC]; 
const result=counterReducer.reduce(function(actionType,counter){ 
   if(INC){ 
       actionType=actionType+1; 
   }
   if(DEC){ 
        actionType=actionType-1; 
   }
        return counter(actionType); 
    
},[]); 
