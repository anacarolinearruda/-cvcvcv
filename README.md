# -cvcvcv


+-------------------------------------+
|            Reembolso               |
+-------------------------------------+
| - id_reembolso: int                 |
| - data_solicitacao: datetime       |
| - status: string                    |
| - valor: float                      |
| - comentarios: string              |
+-------------------------------------+
| + adicionarComentario(comentario: string): void |
| + alterarStatus(novo_status: string): void    |
+-------------------------------------+

+-------------------------------------+
|            Colaborador             |
+-------------------------------------+
| - id_colaborador: int               |
| - nome: string                      |
| - email: string                     |
+-------------------------------------+
| + enviarSolicitacao(reembolso: Reembolso): void |
+-------------------------------------+

+-------------------------------------+
|             Gestor                 |
+-------------------------------------+
| - id_gestor: int                    |
| - nome: string                      |
| - email: string                     |
+-------------------------------------+
| + analisarSolicitacao(reembolso: Reembolso): void |
| + aprovarSolicitacao(reembolso: Reembolso): void |
| + rejeitarSolicitacao(reembolso: Reembolso): void |
+-------------------------------------+

+-------------------------------------+
|        TecnicoAdministrativo        |
+-------------------------------------+
| - id_tecnico: int                   |
| - nome: string                      |
| - email: string                     |
+-------------------------------------+
| + validarSolicitacao(reembolso: Reembolso): void |
+-------------------------------------+
