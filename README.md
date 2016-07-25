In order to run itr with sealights on your computer
You need to change :

<jMeterProcessJVMSettings>
                <arguments>
                  <argument>-Dsl.log.enabled=true</argument>
                  <argument>-Dsl.log.level=INFO</argument>
                  <argument>-Dsl.log.toConsole=true</argument>
                  <argument>-Dsl.pathToMetaJson=&quot;C:\Users\shahar\AppData\Local\Temp\MavenExample_512eaa30-f448-45e7-b86c-cefabcc47b5a.json&quot;</argument>
                  <argument>-Dsl.includes=&quot;*edu.lmu.*&quot;</argument>
                  <argument>-Dsl.branchName=&quot;origin/master&quot;</argument>
                  <argument>-Dsl.buildName=&quot;76&quot;</argument>
                  <argument>-Dsl.environmentName=&quot;Performance&quot;</argument>
                  <argument>-Dsl.moduleName=&quot;MavenExample&quot;</argument>
                  <argument>-Dsl.appName=&quot;MavenExample&quot;</argument>
                  <argument>-Dsl.proxy=&quot;http://127.0.0.1:8888&quot;</argument>
                  <argument>-Dsl.server=&quot;http://52.50.240.57:8080/api&quot;</argument>
                  <argument>-Dsl.customerId=&quot;mod&quot;</argument>
                  <argument>-javaagent:C:\Users\shahar\workspace\sealights\SL.OnPremise.Agents.Java\java-agent-bootstrapper\target\java-agent-bootstrapper-1.0.0-SNAPSHOT.jar</argument>
                </arguments>
</jMeterProcessJVMSettings>

to match your environment (e.g change the path to the agent...).