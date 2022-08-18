
><span style="color: #E11111">org.junit.platform.launcher.core.EngineDiscoveryOrchestrator lambda$logTestDescriptorExclusionReasons$7
INFO: 0 containers and 1 tests were Method or class mismatch<span>

&nbsp;&nbsp;Junit5로 테스트 실행시 테스트는 정상적으로 통과하나 로그에 위와 같은 메시지가 뜰 때가 있다. 일단 파악한 바로는 메서드가 아닌 테스트 클래스 전체를 실행해주거나 테스트 빌드 도구를 gradle에서 intellij로 바꿔주면 이 메시지가 뜨지 않고 테스트가 실행된다. gradle로 빌드 시에 실행되지 않는 테스트 메서드가 있다는 걸 알려주는 메시지로 보인다.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIwMzQ1NzMxOCw5Nzc1NDg1OV19
-->