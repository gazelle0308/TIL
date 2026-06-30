# TIL
#### 6월 29일 
- C언어 자유 과제: C언어에 대한 리마인드를 겸하는 시간을 가지게 되었다.


    #include <stdio.h>

    int main(void)
    {
        
        int LoopNum = 0;
        int InNum = 0;
        int OutNum = 0;
        
        while ( LoopNum < 5 )//Ex040202: for( LoopNum = 0; LoopNum < 5; ++LoopNum )
        {
            
            scanf( "%d", &InNum );
            OutNum = OutNum + InNum;
            ++LoopNum; //Ex040202시 제거
            
        }
        printf( "%d\n", OutNum );
        //Ex040102: 누적합
        
        LoopNum = 0;
        InNum = 0;
        OutNum = 1;
        
        while ( LoopNum < 5 )//Ex040203: for( LoopNum = 0; LoopNum < 5; ++LoopNum )
        {
            
            scanf( "%d", &InNum );
            OutNum = OutNum * InNum;
            ++LoopNum; //Ex040203시 제거
            
        }
        printf( "%d\n", OutNum );
        //Ex040103: 누적곱
        
        LoopNum = 1;
        InNum = 0;

        scanf( "%d", &OutNum );
        while ( LoopNum < 5 )//Ex040204: for( LoopNum = 0; LoopNum < 5; ++LoopNum )
        {
            
            scanf( "%d", &InNum );
            OutNum = (OutNum <= InNum) ? InNum : OutNum;
            ++LoopNum; //Ex040204시 제거
            
        }
        printf( "%d\n", OutNum );
        //Ex040104: 최대값	
        
        LoopNum = 1;
        InNum = 0;
        
        scanf( "%d", &OutNum );
        while ( LoopNum < 5 )//Ex040205: for( LoopNum = 0; LoopNum < 5; ++LoopNum )
        {
            
            scanf( "%d", &InNum );
            OutNum = (OutNum >= InNum) ? InNum : OutNum;
            ++LoopNum; //Ex040205시 제거
            
        }
        printf( "%d\n", OutNum );
        //Ex040105: 최소값
        
        OutNum = 1;
        for( int LoopNumF = 0; LoopNumF < 4; ++LoopNumF )
        {
            
            for( int LoopNumS = 0; LoopNumS < 4; ++LoopNumS )
            {
                
                printf( "%d ", OutNum++ );
            
            }
            
            printf( "\n");
            
        }//Ex040503
        
        return 0;
    }

    해당 코드는 변수 선언을 최대한 적게 활용하면서 잦은 초기화를 통하여 미미하나 메모리 사용을 최대한 줄여 조금이나마 쾌적한 프로그래밍을 하기 위한 코드이다.

    초반 최소값과 최대값 문제에서 OutNum을 0으로 초기화하여 상황에 따라 컴파일러 에러가 발생할 수 있었으나, 이에 대하여 발견하고 고민 끝에 첫 입력값 자체를 OutNum에 입력 함으로써 문제를 해결하였다.
  
- 언리얼 블루프린트 개발: 언리얼 엔진을 설치하고 블루프린트를 활용하는 1일차 수업을 듣고 프로젝트 만드는 법, 팹의 활용 방법, 블루프린트의 활용법에 대하여 배웠다.


#### 6월 30일 

 - 언리얼 블루프린트 개발(라이브 세션): 2일차 및 3일차 수업 진도를 따라잡았습니다.
  - 입력 데이터 중계에 대한 블루프린트: <img width="534" height="152" alt="image" src="https://github.com/user-attachments/assets/818b1980-edd2-438d-8c7b-3daae34e8280" />
  - 움직임 제어에 대한 블루프린트: <img width="671" height="211" alt="image" src="https://github.com/user-attachments/assets/0ee8824f-f781-476d-85f5-178bbdedeef7" />
  - 시야 움직임 제어에 대한 블루프린트: <img width="654" height="198" alt="image" src="https://github.com/user-attachments/assets/c709c06c-7e64-421a-b6cf-ec255b3aa8b9" />
  - 조준에 대한 블루프린트: <img width="1008" height="353" alt="image" src="https://github.com/user-attachments/assets/97421206-59ed-41ee-9f3a-f4c1aa5a3e7a" />

  
 - 게임개발종합반(VOD): 1-8까지 진행했습니다.
  - 3인칭 상황에 더 적합한 제어 블루프린트:<img width="802" height="391" alt="image" src="https://github.com/user-attachments/assets/b1e5924c-deff-4983-bbad-d54ad0f5090a" />

