# Unity Extension
자주 사용하는 확장 메소드 및 기능을 아카이빙합니다.

## script description
### ColorExtension.cs
> 코드를 color로 반환

### ComponentExtension.cs
> getComponent 함수를 옵션별로 세분화하여 기능 확장
> ![image](https://github.com/user-attachments/assets/6d4f5417-9544-4fa6-b49c-409b48e75b85)
> - GetOrAddComponent : component를 가져오거나 추가
>
> #### ( NonRecursive, Recursive, Tag요소 3가지로 나누어 확장 )
> #### Find NonRecursive  
>   - GetComponentsOnlyInChildren_NonRecursive : 직계 하위 오브젝트에서만 컴포넌트를 검색 후 배열 반환
>   - GetComponentOnlyInChildren_NonRecursive : 직계 하위 오브젝트에서만 컴포넌트를 검색 후 요소 반환
> #### Find Recursive
>   - GetComponentsOnlyInChildren_Recursive : 모든 하위 오브젝터에서 컴포넌트 배열로 반환
> #### Find With Tag
>   - GetComponentsOnlyInChildrenWithTag_Recursive : recursive하게 Tag요소로 컴포넌트 검색 후 배열 반환
>   - GetComponentOnlyInChildrenWithTag_Recursive : recursive하게 Tag요소로 컴포넌트 검색 후 요소 반환

### UtilityExtensions.cs
> 그 외 자주쓰는 기능
>
> - Remap : 숫자 범위 재매핑
> - ResizeTexture : texture2D 사이즈 조정

### SingletonBehaviour.cs
> 싱글톤 패턴 추상 클래스
>
> 제너릭으로 인스턴스를 고정합니다
>   - Awake : 생성 시 인스턴스 할당
>   - Instance : 인스턴스 반환 프로퍼티, null일 경우 생성 후 반환
