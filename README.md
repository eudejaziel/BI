INSERT INTO ESTADO (COD_ESTADO,NOME_ESTADO)VALUES (1,'MINAS GERAIS')
INSERT INTO ESTADO (COD_ESTADO,NOME_ESTADO)VALUES (2,'RIO DE JANEIRO')
INSERT INTO ESTADO (COD_ESTADO,NOME_ESTADO)VALUES (3,'SAO PAULO');
INSERT INTO ESTADO (COD_ESTADO,NOME_ESTADO)VALUES (4,'RIO GRANDE NORTE')

INSERT INTO CIDADE (COD_CIDADE,COD_ESTADO,NOME_CIDADE)VALUES (1,1,'BELO HORIZONTE');
INSERT INTO CIDADE (COD_CIDADE,COD_ESTADO,NOME_CIDADE)VALUES (2,2,'CABO FRIO');
INSERT INTO CIDADE (COD_CIDADE,COD_ESTADO,NOME_CIDADE)VALUES (3,3,'CAMPINAS');
INSERT INTO CIDADE (COD_CIDADE,COD_ESTADO,NOME_CIDADE)VALUES (4,4,'NATAL');

INSERT INTO BAIRRO (COD_BAIRRO,COD_CIDADE,NOME_BAIRRO)VALUES (1,1,'TUPI B');
INSERT INTO BAIRRO (COD_BAIRRO,COD_CIDADE,NOME_BAIRRO)VALUES (2,2,'BOTAFOGO');
INSERT INTO BAIRRO (COD_BAIRRO,COD_CIDADE,NOME_BAIRRO)VALUES (3,3,'MORUMBI');
INSERT INTO BAIRRO (COD_BAIRRO,COD_CIDADE,NOME_BAIRRO)VALUES (4,4,'GARCIAS');

INSERT INTO TIPO_ENDERECO(COD_TIPO,NOME_TIPO) VALUES(1,'RESIDENCIAL');
INSERT INTO TIPO_ENDERECO(COD_TIPO,NOME_TIPO) VALUES(2,'COMERCIAL');
INSERT INTO TIPO_ENDERECO(COD_TIPO,NOME_TIPO) VALUES(3,'RURAL');

INSERT INTO ENDERECO(COD_ENDERECO,COD_TIPO,COD_BAIRRO,RUA,NUMERO) VALUES(1,1,1,'ALFEU DE CARVALHO',123);
INSERT INTO ENDERECO(COD_ENDERECO,COD_TIPO,COD_BAIRRO,RUA,NUMERO) VALUES(2,2,1,'NELSON HUNGRIA',43);
INSERT INTO ENDERECO(COD_ENDERECO,COD_TIPO,COD_BAIRRO,RUA,NUMERO) VALUES(3,3,1,'SARAMENHA',52);
INSERT INTO ENDERECO(COD_ENDERECO,COD_TIPO,COD_BAIRRO,RUA,NUMERO) VALUES(4,3,2,'PEDRO ALVES',32);

INSERT INTO ESPECIALIDADE(COD_ESPECIA,NOME_ESPECIA) VALUES (1,'ORTONTODIA');
INSERT INTO ESPECIALIDADE(COD_ESPECIA,NOME_ESPECIA) VALUES (2,'OTORRINO');
INSERT INTO ESPECIALIDADE(COD_ESPECIA,NOME_ESPECIA) VALUES (3,'FISIOTERAPEUTA');
INSERT INTO ESPECIALIDADE(COD_ESPECIA,NOME_ESPECIA) VALUES (4,'CARDIOLOGISTA');

INSERT INTO MEDICO (CRM,COD_ESPECIA,NOME_MEDICO)VALUES(1234,1,'ARTUR NEIVA');
INSERT INTO MEDICO (CRM,COD_ESPECIA,NOME_MEDICO)VALUES(1721,2,'FLAVIA MARIA');
INSERT INTO MEDICO (CRM,COD_ESPECIA,NOME_MEDICO)VALUES(8998,3,'JOSE ELISIO');
INSERT INTO MEDICO (CRM,COD_ESPECIA,NOME_MEDICO)VALUES(6754,4,'GIOVANI SILVA');

INSERT INTO DIAGNOSTICO(CID,DESC_DIAGNOSTICO) VALUES (1,'DOR DE CABEÇA');
INSERT INTO DIAGNOSTICO(CID,DESC_DIAGNOSTICO) VALUES (2,'DENGUE');
INSERT INTO DIAGNOSTICO(CID,DESC_DIAGNOSTICO) VALUES (3,'CANCER');
INSERT INTO DIAGNOSTICO(CID,DESC_DIAGNOSTICO) VALUES (4,'ANEMIA');

INSERT INTO MEDICAMENTO (COD_MEDICAMENTO,NOME_MEDICA,VLR_MEDICA)VALUES(1,'AFINITOR',12);
INSERT INTO MEDICAMENTO (COD_MEDICAMENTO,NOME_MEDICA,VLR_MEDICA)VALUES(2,'ALIMTA',43);
INSERT INTO MEDICAMENTO (COD_MEDICAMENTO,NOME_MEDICA,VLR_MEDICA)VALUES(3,'SIMULECT',90);
INSERT INTO MEDICAMENTO (COD_MEDICAMENTO,NOME_MEDICA,VLR_MEDICA)VALUES(4,'ZOLADEX LA',19);

INSERT INTO EXAME (COD_EXAME,NOME_EXAME,VLR_EXAME) VALUES (1,'URINA',123);
INSERT INTO EXAME (COD_EXAME,NOME_EXAME,VLR_EXAME) VALUES (2,'HEMOGLOBINA',123);
INSERT INTO EXAME (COD_EXAME,NOME_EXAME,VLR_EXAME) VALUES (3,'RESSONANCIA MAGNETICA',123);
INSERT INTO EXAME (COD_EXAME,NOME_EXAME,VLR_EXAME) VALUES (4,'FEZES',123);

INSERT INTO PROCEDIMENTO (COD_PROCED,NOME_PROCED,VLR_PROCED)VALUES (1,'CONSULTA MEDICA',100);
INSERT INTO PROCEDIMENTO (COD_PROCED,NOME_PROCED,VLR_PROCED)VALUES (2,'ASSISNTENCIA AO RECEM-NASCIDO',250);
INSERT INTO PROCEDIMENTO (COD_PROCED,NOME_PROCED,VLR_PROCED)VALUES (3,'ELETROMIOGRAFIA',700);
INSERT INTO PROCEDIMENTO (COD_PROCED,NOME_PROCED,VLR_PROCED)VALUES (4,'COLONOSCOPIA ',450);

INSERT INTO PLANO_SAUDE(COD_PLANO,NOME_PLANO)VALUES(1,'BRADESCO');
INSERT INTO PLANO_SAUDE(COD_PLANO,NOME_PLANO)VALUES(2,'CASSI');
INSERT INTO PLANO_SAUDE(COD_PLANO,NOME_PLANO)VALUES(3,'FORLUZ');
INSERT INTO PLANO_SAUDE(COD_PLANO,NOME_PLANO)VALUES(4,'SUL-AMERICA');

INSERT INTO PACIENTE(COD_PACIENTE,COD_PLANO,COD_ENDERECO,NOME_PACIENTE) VALUES(1,1,1,'EUDE');
INSERT INTO PACIENTE(COD_PACIENTE,COD_PLANO,COD_ENDERECO,NOME_PACIENTE) VALUES(2,2,2,'MARIA');
INSERT INTO PACIENTE(COD_PACIENTE,COD_PLANO,COD_ENDERECO,NOME_PACIENTE) VALUES(3,3,3,'JOSE');
INSERT INTO PACIENTE(COD_PACIENTE,COD_PLANO,COD_ENDERECO,NOME_PACIENTE) VALUES(4,4,4,'ALFREDO');

INSERT INTO CONSULTA(COD_CONSULTA,COD_PACIENTE,COD_PLANO,CRM,CID,DATA_CONSULTA,VLR_CONSULTA,DESC_SINTOMA)
VALUES (1,1,1,6754,1,'27/09/2015',129,'MUITA DOR DE CABEÇA');

INSERT INTO CONSULTA(COD_CONSULTA,COD_PACIENTE,COD_PLANO,CRM,CID,DATA_CONSULTA,VLR_CONSULTA,DESC_SINTOMA)
VALUES (2,2,2,1721,2,'28/09/2015',129,'FEBRE ALTA, VOMITO E SANGRAMENTO');

INSERT INTO CONSULTA(COD_CONSULTA,COD_PACIENTE,COD_PLANO,CRM,CID,DATA_CONSULTA,VLR_CONSULTA,DESC_SINTOMA)
VALUES (3,3,3,1234,1,'29/09/2015',129,'PÉ QUEBRADO E LUXAÇÃO');

INSERT INTO CONSULTA(COD_CONSULTA,COD_PACIENTE,COD_PLANO,CRM,CID,DATA_CONSULTA,VLR_CONSULTA,DESC_SINTOMA)
VALUES (4,4,4,6754,1,'30/09/2015',129,'RETINA QUEBRADA');

INSERT INTO EXAME_CONSULTA(COD_CONSULTA,COD_EXAME,QDTE_EXAME)VALUES(1,1,1);
INSERT INTO EXAME_CONSULTA(COD_CONSULTA,COD_EXAME,QDTE_EXAME)VALUES(2,2,5);
INSERT INTO EXAME_CONSULTA(COD_CONSULTA,COD_EXAME,QDTE_EXAME)VALUES(3,3,12);
INSERT INTO EXAME_CONSULTA(COD_CONSULTA,COD_EXAME,QDTE_EXAME)VALUES(4,4,45);

INSERT INTO MEDICAMENTO_CONSULTA(COD_MEDICAMENTO,COD_CONSULTA,QTDE_MEDICA) VALUES(1,1,34);
INSERT INTO MEDICAMENTO_CONSULTA(COD_MEDICAMENTO,COD_CONSULTA,QTDE_MEDICA) VALUES(2,2,44);
INSERT INTO MEDICAMENTO_CONSULTA(COD_MEDICAMENTO,COD_CONSULTA,QTDE_MEDICA) VALUES(3,3,65);
INSERT INTO MEDICAMENTO_CONSULTA(COD_MEDICAMENTO,COD_CONSULTA,QTDE_MEDICA) VALUES(4,4,78);

INSERT INTO PROCEDIMENTO_CONSULTA(COD_PROCED,COD_CONSULTA,QTDE_PROCED)VALUES(1,1,1);
INSERT INTO PROCEDIMENTO_CONSULTA(COD_PROCED,COD_CONSULTA,QTDE_PROCED)VALUES(2,2,15);
INSERT INTO PROCEDIMENTO_CONSULTA(COD_PROCED,COD_CONSULTA,QTDE_PROCED)VALUES(3,3,34);
INSERT INTO PROCEDIMENTO_CONSULTA(COD_PROCED,COD_CONSULTA,QTDE_PROCED)VALUES(4,4,33);


INSERT INTO MATERIAL (COD_MATERIAL,NOME_MATERIAL,VLR_MATERIAL) VALUES(1,'BISTURI',45);
INSERT INTO MATERIAL (COD_MATERIAL,NOME_MATERIAL,VLR_MATERIAL) VALUES(2,'AGULHA',67);
INSERT INTO MATERIAL (COD_MATERIAL,NOME_MATERIAL,VLR_MATERIAL) VALUES(3,'GAZINHA',88);
INSERT INTO MATERIAL (COD_MATERIAL,NOME_MATERIAL,VLR_MATERIAL) VALUES(4,'FITA ADESIVA',45);

INSERT INTO PROCEDIMENTO_MATERIAL(COD_PROCED,COD_MATERIAL,QTDE_MATERIAL)VALUES(1,1,23);
INSERT INTO PROCEDIMENTO_MATERIAL(COD_PROCED,COD_MATERIAL,QTDE_MATERIAL)VALUES(2,2,456);
INSERT INTO PROCEDIMENTO_MATERIAL(COD_PROCED,COD_MATERIAL,QTDE_MATERIAL)VALUES(3,3,90);
INSERT INTO PROCEDIMENTO_MATERIAL(COD_PROCED,COD_MATERIAL,QTDE_MATERIAL)VALUES(4,4,234);

