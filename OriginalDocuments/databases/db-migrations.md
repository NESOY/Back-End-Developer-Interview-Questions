# DB 마이그레이션

## [Krzysztof Grzybek](https://github.com/krzysztof-grzybek)

이 전략은 다운타임 가능성에 매우 의존적입니다. 다운타임이 가능하다면, 마이그레이션이 훨씬 쉬워질 것입니다. 특히 다음 사항들을 주의를 기울일 것입니다.
1. 마이그레이션이 시작된 이후 데이터 변경의 일관성 (다운타임이 불가능한 경우)
2. 서로 다른 db 엔진 간의 데이터 타입 호환성
3. 데이터베이스 API 변경
4. 보안 이슈 (네트워크를 통해 많은 민감한 데이터들을 옮길 때)
5. 까다로운 잠재적인 복귀