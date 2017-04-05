#include <iostream>
#include <cstring> 

int main(){
　　char aTemp1[100] = "I'm a programmer.";
　　char *pTemp2 = "I'm a programmer.";
　　char aTemp3[] = "C++ How To Program";

　　cout<<sizeof(aTemp1)<<endl; //출력값 100  // 배열의 크기를 반환. 1byte * 100 = 100
　　cout<<sizeof(pTemp2)<<endl; //출력값 4     // 포인터의 크기는 4byte
　　cout<<sizeof(aTemp3)<<endl; //출력값 19　// 문자열의 길이 + 1 (18 + 1)
　　　　　　　　　　　　　　　　　// 배열의 끝을 알려주는 것은 NULL 문자입니다.
　　　　　　　　　　　　　　　　　// 따라서, 18개의 문자 배열에는 17개밖에 쓰지 못합니다.

　　cout<<strlen(aTemp1)<<endl; //17 모두 실제 문자열의 길이값이 나옵니다.
　　cout<<strlen(pTemp2)<<endl; //17 NULL문자를 제외한 배열의 길이입니다.
　　cout<<strlen(aTemp3)<<endl; //18 글자의 길이
		return 0;
}
	
