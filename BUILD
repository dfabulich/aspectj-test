java_test(
    name='apptest',
    srcs=['src/test/java/com/redfin/AppTest.java'],
    test_class='com.redfin.AppTest',
    deps=['@junit_junit//jar', '@org_hamcrest_hamcrest_core//jar'],
)

java_test(
    name='apptest_weaver',
    srcs=['src/test/java/com/redfin/AppTest.java'],
    test_class='com.redfin.AppTest',
    deps=['@junit_junit//jar', '@org_hamcrest_hamcrest_core//jar', '@org_aspectj_aspectjweaver//jar'],
    jvm_flags=['-javaagent:$(location @org_aspectj_aspectjweaver//jar)'],
)
