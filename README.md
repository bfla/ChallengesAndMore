ChallengesAndMore
=================

Intuit API class


#region Assembly Intuit.Ipp.DataAggregation.Data.dll, v1.5.1.0
// C:\Users\Sully\Documents\Visual Studio 2013\CollabCap\packages\IPPAggCatDotNetDevKit.1.5.1.1\lib\Intuit.Ipp.DataAggregation.Data.dll
#endregion

using System;
using System.CodeDom.Compiler;
using System.ComponentModel;
using System.Diagnostics;
using System.Xml.Serialization;

namespace Intuit.Ipp.DataAggregation.Data
{
    [Serializable]
    [DebuggerStepThrough]
    [DesignerCategory("code")]
    [GeneratedCode("Intuit.Ipp.DataAggregation.XsdExtension", "3.0.0.0")]
    [XmlRoot(Namespace = "http://schema.intuit.com/platform/fdatafeed/challenge/v1", IsNullable = false)]
    [XmlType(AnonymousType = true, Namespace = "http://schema.intuit.com/platform/fdatafeed/challenge/v1")]
    public class Challenges
    {
        public Challenges();

        [XmlElement("challenge")]
        public ChallengesChallenge[] challenge { get; set; }
    }
}

namespace Intuit.Ipp.DataAggregation.Data
{
    [Serializable]
    [DebuggerStepThrough]
    [DesignerCategory("code")]
    [GeneratedCode("Intuit.Ipp.DataAggregation.XsdExtension", "3.0.0.0")]
    [XmlType(AnonymousType = true, Namespace = "http://schema.intuit.com/platform/fdatafeed/challenge/v1")]
    public class ChallengesChallenge
    {
        public ChallengesChallenge();

        [XmlElement("text", typeof(String))]
        public object[] AnyIntuitObjects { get; set; }
        //
        [XmlElement("choice")]
        public ChallengesChallengeChoice[] choice { get; set; }
    }
}

namespace Intuit.Ipp.DataAggregation.AggregationCategorizationServices
{
    // Summary:
    //     Challenge Session Information.
    public class ChallengeSession
    {
        public ChallengeSession();

        // Summary:
        //     Gets or sets the Challenge Node Id Value.
        public string ChallengeNodeId { get; set; }
        //
        // Summary:
        //     Gets or sets the Challenge Session Id Value.
        public string ChallengeSessionId { get; set; }
        //
        // Summary:
        //     Gets or sets the Id value which can be both InstitutionId and InstitutionLoginId.
        public long Id { get; set; }
    }
}

namespace Intuit.Ipp.DataAggregation.Data
{
    [Serializable]
    [DebuggerStepThrough]
    [DesignerCategory("code")]
    [GeneratedCode("Intuit.Ipp.DataAggregation.XsdExtension", "3.0.0.0")]
    [XmlType(AnonymousType = true, Namespace = "http://schema.intuit.com/platform/fdatafeed/challenge/v1")]
    public class ChallengesChallengeChoice
    {
        public ChallengesChallengeChoice();

        public string text { get; set; }
        //
        public string val { get; set; }
    }
}


