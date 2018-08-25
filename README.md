# Internet Explorer browser filtering

### LICENSE

이 프로그램은 [GNU GPL LICENSE](http://korea.gnu.org/documents/copyleft/gpl.ko.html) 를 따릅니다.

### 설명

Internet Explorer browser 를 지원하지 않는 사이트를 위한 Internet Explorer browser 를 걸러내는 사이트입니다.

### 사용법

당신의 사이트의 Html 코드에서 <head> 바로밑에 아래 코드를 삽입하십시오
  
  ```
          <script>var agent = navigator.userAgent.toLowerCase();
                if ( (navigator.appName == 'Netscape' && navigator.userAgent.search('Trident') != -1) || (agent.indexOf("msie") != -1) ) {
                    window.location.href="https://newpremium.github.io/IE_filtering/index.html";
                }
                </script>
  ```
  
