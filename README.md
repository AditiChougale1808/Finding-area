// Online C compiler to run C program online
#include <stdio.h>
#include <string.h>

int main() {
    // Write C code here
    int i,j,pincode;
    int pin[5]={411014,411032,411038,411052,411004};
  char loc[5][30]={"VimanNagar","PuneAirport","Kothrud","Karvenagar","Deccan"};
    int found=0;
    printf("Enter the pincode:");
    scanf("%d",&pincode);

for(i=0;i<5;i++){
     
    if(pincode==pin[i]){
        printf("Pincode: %d\n",pin[i]);
        printf("Area: %s\n",loc[i]);
        printf("Pincode is found.\n");
        found++;
        break;
        }
    }
    if(found==0)
    {
        printf("Pincode not found.");
        
    }
    
        return 0;
    }
