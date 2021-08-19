- 👋 Hi, I’m @yrahul16
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
yrahul16/yrahul16 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include <stdio.h>
int main(){
    int arr[]={1,22,3,44,5};
    int i = 0 , size = 5, ind = 3,item = 10;
    int j = size;
    printf("The original array is \n");
    for(i=0;i<size;i++){
        printf(" %d ",arr[i]);
    }
    printf("\n");
    size = size+1;
    while(j>=ind){
        arr[j+1]= arr[j];
        j = j-1;
    }
    arr[ind]= item;
    printf("The insertion of array is \n");
    for(i=0;i<size;i++){
        printf(" %d ",arr[i]);
    }
    printf("\n");
    j = ind;
    while(j<size){
        arr[j]= arr[j+1];
        j = j+1;
    }
    size = size-1;
    printf("The deletion if array element \n");
    
    for(i=0;i<size;i++){
        printf(" %d ",arr[i]);
    }
    
    return 0;
}
