# Create and configure basic Pods

{% tabs %}
{% tab title="Question 1" %}
Write a command to get a list of all pods.
{% endtab %}

{% tab title="Answer 1" %}
```text
kubectl get pods
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Question 2" %}
create a pod using the latest container image of `nginx`, that expose the port 8080.
{% endtab %}

{% tab title="Answer 2" %}
```text
kubectl run myPod --image=nginx:latest --port=8080
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Question 3" %}
Create a Pod with container image that corresponds to version `1.14.0` of `nginx`
{% endtab %}

{% tab title="Answer 3" %}
```text
kubectl run myPod --image=nginx:1.14.0
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Question 4" %}
Get the address IP of pod named myPod.
{% endtab %}

{% tab title="Answer 4" %}
```text
kubectl describe pod/myPod | grep IP
```
{% endtab %}
{% endtabs %}

