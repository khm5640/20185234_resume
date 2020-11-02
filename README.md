
# 구현 program

## java script
### - 치매 예방 프로그램

''' js

<html>
<body>
<script type= "text/javascript">
	
	var mes,i,res1,res2,suc,fail,wch,yet;

	var a=["체리","포도","딸기","멜론"]; 
 	var b=["아이스아메리카노","유자차","아이스크림","카페라떼"]; 
	var c=["냉면","칼국수","막국수","된장찌개"];

	choice=eval(prompt("  *** 배고픈 물개에게 음식을 줍시다 !! *** \n 주고 싶은 카테고리를 선택해주세요.^^\n 1. 과일 2. 디저트 3. 밥 "),"");
	mes=" ** 분류가 잘못 되면 게임이 종료됩니다. ** \n 준비가 되셨다면 확인을 눌러서 게임을 시작해 주세요~";	

	suc="완벽해요..!!!!!  물개는 이제 행복합니다.^0^";
	fail="틀리셨습니다 ! 게임을 종료 합니다.";
	wch="숫자를 잘못 입력 하셨습니다.. 게임을 종료합니다.";
	yet="준비가 안되셨군요,,, 마음의 준비 하시고 다시 시도 해 주세요. 종료합니다.";

	if(choice==1)
	{
		res=confirm(" [ 과일 ]을 선택 하셨습니다 ! \n  물개는 오직 빨간 과일만을 먹습니다. \n  빨간 과일이 나오면 확인을,  그 외의 것이 나오면\n 취소를 눌러서 과일을 분류해주세요^^\n  " + mes);
	              if(res==true)
		{
			for(i=0;i<4;i++)
			{
				if(i%2==0)
					res1=confirm(a[i]);
				else
					res2=confirm(a[i]);
			}

		       if(res1==true && res2==false)
	                     {
			document.write(suc);
	                      }

		       else
			document.write(fail);
			
	
		}	
		else
		   document.write(yet);
	
		
	}




	else if(choice==2)
	{
		res=confirm(" [ 디저트 ]를 선택 하셨습니다 ! \n  물개는 오직 차가운 것만을 먹습니다.\n  차가운 것이 나오면 확인을,  그 외의 것이 나오면\n 취소를 눌러서 디저트를 분류해주세요^^\n  " + mes);
	              if(res==true)
		{
			for(i=0;i<4;i++)
			{
				if(i%2==0)
					res1=confirm(b[i]);
				else
					res2=confirm(b[i]);
			}

		       if(res1==true && res2==false)
	                     {
			document.write(suc);
	                      }

		       else
			document.write(fail);
			
	
		}	
		else
		   document.write(yet);
	
		
	}


	else if(choice==3)
	{
		res=confirm(" [ 음식 ]을 선택 하셨습니다 ! \n  물개는 오직 따뜻한 음식만을 먹습니다.\n  따뜻한 것이 나오면 확인을,  그 외의 것이 나오면\n 취소를 눌러서 음식을 분류해주세요^^\n  " + mes);
	              if(res==true)
		{
			for(i=0;i<4;i++)
			{
				if(i%2==1)
					res1=confirm(c[i]);
				else
					res2=confirm(c[i]);
			}

		       if(res1==true && res2==false)
	                     {
			document.write(suc);
	                      }

		       else
			document.write(fail);
			
	
		}	
		else
		   document.write(yet);
	
		
	}

	else
		document.write(wch)

   </script>
  </body>
 </html>
 '''