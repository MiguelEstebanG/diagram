Example of mermaid diagram

```mermaid
graph TD;

    ceo(
        Martín Mieres
        <b> Chief Executive Officer </b>
    ) ----- areaDeMarketing

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


    ceo(
        Martín Mieres
        <b> Chief Executive Officer </b>
    );

    subgraph departamentodeMarketing[ ]
        areaDeMarketing((<b> Área de Marketing </b>))

        subgraph departamentoDeComunicacion[ ]
            dptoComunicacion[<b> Departamento de Comunicación </b>]
            directorDeComunicacion(
                Marcos Pérez
                <b> Director de comunicación </b>
            )
            communityManager([
                Carlos Sánchez
                <b> Community manager </b>
            ])
            becario1([
                Diego López
                <b> Becario </b>
            ])
        end
        
        subgraph departamentoDePublicidad[ ]
            dptoPublicidad[<b> Departamento de Publicidad </b>]
            directorDePublicidad(
                Javier Férnandez
                <b> Director de Publicidad </b>
            )
            directorCreativo([
                Carlos Sánchez
                <b> Director Creativo </b>
            ])
            becario2([
                Diego López
                <b> Becario </b>
            ])
        end

    end

    subgraph departamentodeNegocio[ ]
        areaDeNegocio((<b> Área de Negocio </b>))

        subgraph departamentoDeProduccion[ ]
            dptoProduccion[<b> Departamento de Produccion </b>]
            jefeDeProduccion(
                Carla Pérez
                <b> Jefe de Producción </b>
            )
            trabajador([
                José López
                <b> Trabajador en fábrica </b>
            ])
        end
        
        subgraph departamentoFinanciero[ ]
            dptoFinanciero[<b> Departamento Financiero </b>]
            gestoria(
                Gestor X
                <b> Gestoría Externa </b>
            )
        end

        subgraph departamentoDeVentas[ ]
            dptoVentas[<b> Departamento de Ventas </b>]
            directorComercial(
                Fernando Vázquez
                <b> Director Comercial </b>
            )
            jefeDeVentas([
                Pedro García
                <b> Jefe de Ventas </b>
            ])
            comercial([
                María Díaz
                <b> Comercial </b>
            ])
        end

    end

    linkStyle default stroke-width: 1px;

```
