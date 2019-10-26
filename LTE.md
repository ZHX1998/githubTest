struct ReportBufferStatusParameters  
  {  
    uint16_t rnti;  /**< the C-RNTI identifying the UE */  
    uint8_t lcid;  /**< the logical channel id corresponding to the sending RLC instance */  
    uint32_t txQueueSize;  /**< the current size of the RLC transmission queue */  
    uint16_t txQueueHolDelay;  /**< the Head Of Line delay（排头阻塞） of the transmission queue */  
    uint32_t retxQueueSize;  /**<  the current size of the RLC retransmission queue in bytes */  
    uint16_t retxQueueHolDelay;  /**<  the Head Of Line delay of the retransmission queue */  
    uint16_t statusPduSize;  /**< the current size of the pending STATUS RLC  PDU message in bytes */  
    /* Additional identifier for sidelink */（源id和目的id，一对多的关系）  
    uint32_t srcL2Id;  /**< Source L2 ID (24 bits) */  
    uint32_t dstL2Id;  /**< Destination L2 ID (24 bits) */  
  };  

