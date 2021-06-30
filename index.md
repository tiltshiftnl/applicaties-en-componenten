---
---
<br>
{% for item in site.data.applicaties-en-componenten %}
<h2>{{ item.familie }}</h2>
<p>{{ item.context }}</p>
<table>
    <tr>
        <th>naam</th>
        <th>omschrijving</th>
        <th>gebruiker</th>
        <th>type</th>
        <th>gebruikslocatie</th>
    </tr>
    {% for applicatie in item.applicaties %}
    <tr>
        <td style="font-weight: 900">{{ applicatie.naam }}</td>
        <td>{{ applicatie.omschrijving }}</td>
        <td>{{ applicatie.gebruiker }}</td>
        <td>{{ applicatie.type }}</td>
        <td>{{ applicatie.gebruikslocatie }}</td>
    </tr>
    {% endfor %}
</table>
{% endfor %}
