


**@Transactional 어노테이션을 이용한 트랜잭션 적용**

 - Mybatis 설정 클래스 파일에 추가
 - Transaction을 사용하기 위한 설정
   
   

   

	     @Bean
	        public DataSourceTransactionManager transactionManager(){
	    	    return new DataSourceTransactionManager(DataSource());
	    	}


 - 서비스 레이어에서 @Transactional 어노테이션 적용
 - 메소드 뿐 아니라 인터페이스, 클래스에도 선언 가능
 
		   @Service
		**@Transactional**
		public class UserServiceImpl implements UserService{
		...
		}

ddd
 - 메소드 뿐 아니라 인터페이스, 클래스에도 선언 가능



<!--stackedit_data:
eyJoaXN0b3J5IjpbNjYxMzk0MDE3XX0=
-->
