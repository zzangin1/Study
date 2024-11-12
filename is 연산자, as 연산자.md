코드에서 종종 보이는 연산자라 각 기능을 정확히 이해하고자 정리하게 되었다.

# is 연산자
## 1. 코드
```cs
TcpListener m_server = new TcpListener(9999);
TcpClient m_client = new TcpClient();

var server = m_server is TcpListener;
var client = m_client is TcpClient;
```

## 2. 기능
캐스팅이 가능하면 true 리턴
캐스팅이 불가능하면 false 리턴

캐스팅 성공 유무만 판단할 수 있다.

# as 연산자
## 1. 코드
```cs
TcpListener m_server = new TcpListener(9999);
TcpClient m_client = new TcpClient();

var server = m_server as TcpListener;
var client = m_client as TcpClient;
```

## 2. 기능
캐스팅에 성공하면 캐스팅 타입 리턴
캐스팅에 실패하면 null 리턴

as 연산자는 Reference Type 간의 캐스팅만 가능하다.
