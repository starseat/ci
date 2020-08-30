* CodeIgniter 의 주소체계 - http://호스트/컨트롤러/메서드
* application/config/routes.php 에서 default_controller를 welcome.php로 지정해서 컨트롤러는 알 수 있지만 실행되는 메서드명은 알 수 없음.
* controllers/Welcome.php 처럼 index() 메서드를 선언하면 http://localhost/welcome/ 까지만 수소를 쳐도 자동으로 http://localhost/welcome/ index라고 실행됨.
* 에러 방지의 목적도 있기 때문에 index() 메서드는 항상 만드는 것이 좋음.
  
* index() 의 $this->load->view('welcome_message'); 는 뷰 파일을 로딩하라는 의미이며 application/views/welcome/message.php 파일이 로딩됨. (확장자 생략)