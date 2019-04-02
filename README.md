# ReflectUtil
Wrapper and extension of `java.lang.reflect`.<br/>

Features:
 * Get all fields information of specified object.
 * Get definition name string of specified class field.
 
for example:
<pre><code>
class Test {
    public final static String MODE_AAA = "aaa";
    public final static int EVENT_BBB = 123;
    public final static long MASK_CCC = 0xabcd;
}
<code></pre>
<pre><code>ReflectUtil.getFieldName(Test.class, "aaa")</code></pre> will return "MODE_AAA";<br/>
<pre><code>ReflectUtil.getFieldName(Test.class, 123)</code></pre> will return "EVENT_BBB";<br/>
<pre><code>ReflectUtil.getFieldName(Test.class, 0xabcd)</code></pre> will return "MASK_CCC".<br/>
