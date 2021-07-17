  def를 사용하여 이중탐색을 시도하였다. 
  그런데 숫자를 입력할 때 typeerror와 valueerror가 계속 발생한다.
gaesu = int(input())
numbers = [input().split()]
numbers = list(map(int, numbers))
numbers.sort()
m = int(input())
해당 오류가 계속해서 발생하는 이유를 도저히 모르겠다.
TypeError: int() argument must be a string, a bytes-like object or a number, not 'list' 라는데, map함수를 쓸 때 문제가 생긴 듯 하다.

\2512, 1477, 3079번 모두 동일한 문구가 뜨는 것으로 보아 모두 동일한 부분에서 틀린 것으로 생각된다.
6시까지 가능하면 고쳐
