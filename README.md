% mvn test
% grep "system-out" target/surefire-reports/TEST-SurefireTest.xml 
    <system-out><![CDATA[Test-test?
]]></system-out>
%

but

% mvn test -Dsurefire.rerunFailingTestsCount=1
% grep "system-out" target/surefire-reports/TEST-SurefireTest.xml
%