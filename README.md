# Sunflower 프로젝트 패키지 구조

## [Sunflower 프로젝트](https://github.com/android/sunflower)

![image](https://user-images.githubusercontent.com/48902047/149451934-a5124d6d-f41f-4faf-8995-505a739b86ab.png)
## 프로젝트 패키지 구조
![image](https://user-images.githubusercontent.com/48902047/149452193-b1235a0b-66fc-4566-a7a1-fd8fdace1179.png)
  
## res 구조
![image](https://user-images.githubusercontent.com/48902047/149452231-51f959e8-63b5-4deb-a03c-625d0c35c44c.png)
1. adapter
- 데이터 바인딩에 사용되는 BindingAdapter 가 있습니다.
- 리사이클러뷰 관련 PagingAdapter, ListAdapter 가 있습니다.
- ViewPager2 에 사용할 FragmentStateAdapter 가 있습니다.
2. api
- 외부 서버 API 통신을 위한 인터페이스가 있습니다.
3. data
- Room DataBase 를 사용한 DB 관련 클래스가 들어있습니다.
- Repository 클래스가 들어있습니다.
4. di
- Hilt를 사용한 의존성 주입 모듈들이 들어있습니다.
5. utils
- 유틸성 클래스들인 상수와 latitude(위도)를 구하는 함수가 있는 클래스가 있습니다.
6. viewmodels
- Hilt 의존성 주입 및 코루틴 Flow 로 구현 되어있는 ViewModel 클래스들이 들어습니다.
7. views
- 커스텀한 CardView가 들어있습니다.
8. workers
- WorkManager 관련 클래스인 CoroutineWorker 클래스가 들어있습니다. 데이터베이스 작업에 사용하는 것 같다. CoroutineWorker는 WorkManager를 코루틴과 엮어 더 사용하기 편리하게 한거라고 합니다.
9. 최상위 패키지(루트)
- Jetpack Navigation을 이용한 SPA 구조이므로 하나의 액티비티와 여러개의 프래그먼트들이 들어있습니다.
