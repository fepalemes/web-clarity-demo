# Exemplo de utilização do Microsoft Clarity no Next.JS

Veja como é simples realizar a configuração do Clarity no Next.JS.

## 🚀 Como utilizar

**Configuração no arquivo Layout.tsx**

A forma mais simples de utilizar é adicionar o script no seu layout principal (app/layout.tsx ou app/layout.js).

Troque o XXXXXXX pelo ID do seu projeto no Clarity.

```tsx
<Script id="clarity-script" strategy="afterInteractive">
  {`
  (function(c,l,a,r,i,t,y){
        c[a]=c[a]||function(){(c[a].q=c[a].q||[]).push(arguments)};
        t=l.createElement(r);t.async=1;t.src="https://www.clarity.ms/tag/"+i;
        y=l.getElementsByTagName(r)[0];y.parentNode.insertBefore(t,y);
    })(window, document, "clarity", "script", "XXXXXXX");
  `}
</Script>
  );
}
```

