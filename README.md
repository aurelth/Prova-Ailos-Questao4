"# Prova-Ailos-Questao4"

SELECT 
    ASSUNTO,
    ANO,
    COUNT(*) AS QUANTIDADE
FROM 
    ATENDIMENTOS
GROUP BY 
    ASSUNTO, ANO
HAVING 
    COUNT(*) > 3
ORDER BY 
    ANO DESC, QUANTIDADE DESC;
