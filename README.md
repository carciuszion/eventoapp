# eventoapp
Aplicação Java com Spring boot - cadastro de eventos https://eventoapp-carcius.herokuapp.com/

ALTER TABLE evento_convidados
  ADD CONSTRAINT fkevento1 FOREIGN KEY (evento_codigo) REFERENCES evento (codigo),
  ADD CONSTRAINT fkconvidado1 FOREIGN KEY (convidados_rg) REFERENCES convidado (rg);
  
 ALTER TABLE convidado
  ADD CONSTRAINT fkevento FOREIGN KEY (evento_codigo) REFERENCES evento (codigo)
  
  ALTER TABLE evento_convidados ADD CONSTRAINT vendas_fk FOREIGN KEY (cod_produtos) REFERENCES produtos (codigo);
  
  
  ALTER TABLE convidado ADD CONSTRAINT convidado_pk PRIMARY KEY (rg);
