# matches

int main(void) {
	int t,n1,n2,num, sum,s2;
	scanf("%d", &t);
	while(t--){
	    scanf("%d %d", &n1,&n2);
	    sum=n1+n2;
	    while(sum!=0){
	        num=sum%10;
	    if(num==0|| num==9||num==6){
	        s2= s2+6;
	    }
	    else if(num==1){
	        s2= s2+2;
	    }
	    else if(num==4){
	        s2=s2+4;
	    }
	    else if(num==8){
	        s2= s2+7;
	    }
	    else if(num==2||num==3||num==5){
	        s2= s2+5;
	    }
	    else {
	        s2= s2+3;
	        
	    }
	    sum=sum/10;
	    }
	    printf("%d\n", s2);
	    s2=0;
	}
	return 0;
}
