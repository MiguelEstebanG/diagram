Example of mermaid diagram

```mermaid

graph TD;

   %% Definicion de relaciones
    ceo ----- areaDeMarketing

    areaDeMarketing --- dptoComunicacion
    dptoComunicacion --- directorDeComunicacion
    directorDeComunicacion --- communityManager
    communityManager --- becario1

    areaDeMarketing --- dptoPublicidad
    dptoPublicidad --- directorDePublicidad
    directorDePublicidad --- directorCreativo
    directorCreativo --- becario2
    
    ceo ----- areaDeNegocio

    areaDeNegocio --- dptoProduccion
    dptoProduccion --- jefeDeProduccion
    jefeDeProduccion --- trabajador
    
    areaDeNegocio --- dptoFinanciero
    dptoFinanciero --- gestoria

    areaDeNegocio --- dptoVentas
    dptoVentas --- directorComercial
    directorComercial --- jefeDeVentas
    jefeDeVentas --- comercial

    %%% Diseñamos el organigrama

    ceo(Martín Mieres <br><b> Chief Executive Officer </b></br>);

    %% Área de marketing
    subgraph departamentodeMarketing[ ]
        areaDeMarketing((<b> Área de Marketing </b>));

        subgraph departamentoDeComunicacion[ ]
            dptoComunicacion[<b> Departamento de Comunicación </b>];
            directorDeComunicacion(Marcos Pérez <br><b> Director de comunicación </b></br>);
            communityManager([Carlos Sánchez <br><b> Community manager </b></br>]);
            becario1([Diego López <br><b> Becario </b></br>]);
        end
        
        subgraph departamentoDePublicidad[ ]
            dptoPublicidad[<b> Departamento de Publicidad </b>];
            directorDePublicidad(Javier Férnandez <br><b> Director de Publicidad </b></br>);
            directorCreativo([Carlos Sánchez <br><b> Director Creativo </b></br>]);
            becario2([Diego López <br><b> Becario </b></br>]);
        end

    end

    %% Área de negocio
    subgraph departamentodeNegocio[ ]
        areaDeNegocio((<b> Área de Negocio </b>));

        subgraph departamentoDeProduccion[ ]
            dptoProduccion[<b> Departamento de Produccion </b>];
            jefeDeProduccion(Carla Pérez <br><b> Jefe de Producción </b></br>);
            trabajador([José López <br><b> Trabajador en fábrica </b></br>]);
        end
        
        subgraph departamentoFinanciero[ ]
            dptoFinanciero[<b> Departamento Financiero </b>];
            gestoria(Gestor X <br><b> Gestoría Externa </b></br>);
        end

        subgraph departamentoDeVentas[ ]
            dptoVentas[<b> Departamento de Ventas </b>];
            directorComercial(Fernando Vázquez <br><b> Director Comercial </b></br>);
            jefeDeVentas([Pedro García <br><b> Jefe de Ventas </b></br>]);
            comercial([María Díaz <br><b> Comercial </b></br>]);
        end

    end

    linkStyle default stroke-width: 1px;
```

```
